# Análise de Mercado de Videogames 🎮

## Sobre o projeto

Este projeto tem como objetivo analisar o mercado de videogames por meio de dados históricos de vendas, avaliações de usuários e críticos, plataformas, gêneros e preferências regionais.

A análise busca identificar padrões de consumo e tendências comerciais que possam contribuir para o planejamento de campanhas de marketing para 2017, considerando dados do período de 2012 a 2016.

## Objetivos

- Analisar a evolução das vendas de videogames.
- Identificar as plataformas com maior volume de vendas.
- Investigar a relação entre avaliações e vendas.
- Comparar o desempenho dos gêneros de jogos.
- Analisar as diferenças entre América do Norte, Europa e Japão.
- Avaliar a influência da classificação indicativa ESRB.
- Aplicar testes de hipóteses estatísticas.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## Dados utilizados

O conjunto de dados contém inicialmente 16.715 registros e 11 colunas, incluindo:

- Nome do jogo
- Plataforma
- Ano de lançamento
- Gênero
- Vendas por região
- Avaliações da crítica
- Avaliações dos usuários
- Classificação indicativa ESRB

## Etapas do projeto

### 1. Preparação dos dados

- Padronização dos nomes das colunas.
- Tratamento de valores ausentes.
- Conversão dos tipos de dados.
- Tratamento dos valores identificados como `tbd`.
- Verificação da qualidade dos dados.

### 2. Análise exploratória

- Análise da evolução dos lançamentos.
- Comparação das vendas por plataforma.
- Investigação do ciclo de vida das plataformas.
- Análise das vendas por gênero.
- Comparação das preferências regionais.

### 3. Análise estatística

- Correlação entre avaliações e vendas.
- Comparação das avaliações entre plataformas.
- Comparação das avaliações entre gêneros.
- Aplicação de testes t para amostras independentes.

## Principais resultados

### Plataformas

As plataformas com maiores vendas acumuladas no período analisado foram:

| Plataforma | Vendas |
|---|---:|
| PS4 | 314,14 |
| PS3 | 288,79 |
| Xbox 360 | 236,54 |
| Nintendo 3DS | 194,61 |
| Xbox One | 159,32 |

### Avaliações e vendas

Na análise do PlayStation 4, foram identificadas as seguintes correlações:

| Indicador | Correlação |
|---|---:|
| Avaliação da crítica | 0,407 |
| Avaliação dos usuários | -0,032 |

Os resultados indicam uma associação positiva moderada entre as avaliações da crítica e as vendas, enquanto a correlação entre as avaliações dos usuários e as vendas foi praticamente nula.

### Gêneros mais vendidos

| Gênero | Vendas |
|---|---:|
| Action | 441,12 |
| Shooter | 304,73 |
| Role-Playing | 192,80 |
| Sports | 181,07 |
| Misc | 85,04 |

Action e Shooter apresentaram os maiores volumes de vendas acumuladas no período.

### Diferenças regionais

- **América do Norte:** destaque para Xbox 360, Action e Shooter.
- **Europa:** destaque para PS4, Action e Shooter.
- **Japão:** destaque para Nintendo 3DS e Role-Playing.

Os resultados demonstram diferenças nas preferências dos consumidores entre os mercados analisados.

## Testes de hipóteses

Foi utilizado um nível de significância de 5% (`α = 0,05`).

| Comparação | Valor-p | Resultado |
|---|---:|---|
| Xbox One × PC | 0,549 | Não houve evidência suficiente de diferença entre as médias |
| Action × Sports | 4,24 × 10⁻²⁰ | Foi identificada diferença estatisticamente significativa |

## Conclusão

A análise identificou padrões importantes no mercado de videogames, incluindo o desempenho das principais plataformas, a concentração das vendas em determinados gêneros e as diferenças de preferência entre regiões.

Também foi observada uma associação mais forte entre as avaliações da crítica e as vendas do PS4 do que entre as avaliações dos usuários e as vendas.

O projeto demonstra a aplicação de técnicas de análise exploratória, limpeza de dados, visualização, correlação e testes estatísticos para extrair informações relevantes a partir de dados históricos.

## Como executar o projeto

### Pré-requisitos

- Python 3 instalado.
- Jupyter Notebook.
- Arquivo de dados `games.csv`.

### 1. Clone o repositório

```bash
git clone https://github.com/pedroferrarini/video-game-sales-analysis.git
```

### 2. Acesse a pasta do projeto

```bash
cd video-game-sales-analysus
```

### 3. Instale as bibliotecas necessárias

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
```

### 4. Inicie o Jupyter Notebook

```bash
jupyter notebook
```

### 5. Execute a análise

No navegador, abra o notebook `.ipynb` do projeto e execute as células em ordem, começando pela primeira.

**Observação:** o arquivo `games.csv` deve estar disponível no caminho esperado pelo notebook. Caso os dados não estejam no local correto, ajuste o caminho utilizado na leitura do arquivo.

## Competências desenvolvidas

- Análise exploratória de dados (EDA).
- Limpeza e tratamento de dados.
- Manipulação de dados com Pandas.
- Visualização de dados.
- Análise de correlação.
- Testes de hipóteses estatísticas.
- Interpretação de resultados para apoio à tomada de decisão.

---

