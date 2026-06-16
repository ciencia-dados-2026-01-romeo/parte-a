# Projeto I - EDA: Percepção de Desigualdade no Brasil

Parte A da disciplina de Ciência de Dados.

Este repositório reúne os artefatos da análise exploratória sobre percepção de desigualdade no Brasil, usando microdados do IPEC e comparação com dados oficiais do IBGE.

## Sumário das entregas

| Item | Entrega | Arquivo / link | Status |
| --- | --- | --- | --- |
| 2.1 | Notebook executável no Colab com as análises desenvolvidas | [`parte_a.ipynb`](parte_a.ipynb) | Entregue |
| 2.2 | Dados empregados no projeto | [`04839.sav`](04839.sav) | Entregue |
| 2.3 | Texto do trabalho com Introdução, Métodos e Resultados/Conclusão | [`ParteA.docx`](ParteA.docx) | Entregue |
| 2.4 | Vídeo de apresentação, com até 5 minutos | [YouTube](https://www.youtube.com/watch?v=VsmX3hzhics) | Entregue |
| 2.4 | Slides empregados na apresentação | [`Percepcao-de-Desigualdade-no-Brasil.pptx`](Percepcao-de-Desigualdade-no-Brasil.pptx) | Entregue |
| 2.5 | README com sumário das entregas | [`README.md`](README.md) | Entregue |

## Autores

- João Paulo Bonagurio Ramirez - RA: 22.01247-8
- Lucas Olivares Borges da Silva - RA: 22.00889-6
- Luis Gustavo Machado - RA: 21.00322-0
- Tiago Tadeu de Azevedo - RA: 22.00856-0
- Victor Augusto de Gasperi - RA: 22.00765-2

## Tema

O trabalho investiga como a população brasileira percebe a desigualdade social e em quais ambientes essa desigualdade aparece com maior intensidade. A análise considera fatores sociodemográficos, como sexo, raça/cor, escolaridade, renda, região e porte do município.

A base principal é o estudo IPEC 04839, armazenado em formato SPSS (`.sav`). O notebook também consulta dados públicos do IBGE via API para comparar a distribuição por sexo da amostra com dados oficiais.

## Como executar o notebook

1. Abra o arquivo [`parte_a.ipynb`](parte_a.ipynb) no Google Colab.
2. Execute as células em ordem.
3. O notebook instala os pacotes necessários durante a execução:
   - `pyreadstat`
   - `plotly`
   - `seaborn`
   - `requests`
4. A base [`04839.sav`](04839.sav) está no repositório e também é carregada no notebook por URL do GitHub.

## Estrutura do repositório

```text
.
├── 04839.sav       # Base de dados IPEC em formato SPSS
├── ParteA.docx     # Texto do trabalho
├── Percepcao-de-Desigualdade-no-Brasil.pptx # Slides da apresentação
├── README.md       # Sumário e organização das entregas
└── parte_a.ipynb   # Notebook com EDA, visualizações e testes estatísticos
```

## Métodos empregados

A análise foi desenvolvida em Python, com foco em:

- leitura e tratamento de dados em formato `.sav`;
- recategorização de variáveis sociodemográficas;
- análise exploratória de frequências e distribuições;
- visualizações com Matplotlib, Seaborn e Plotly;
- comparação da amostra IPEC com dados públicos do IBGE;
- teste Qui-Quadrado de Independência para avaliar associação entre escolaridade e percepção de locais de desigualdade;
- análises adicionais por renda, região, porte de município e variáveis de percepção.

## Principais resultados

- A amostra do IPEC possui 2.000 registros.
- A distribuição por sexo da amostra ficou próxima dos dados oficiais do IBGE, com desvio inferior a 1 ponto percentual.
- O trabalho identifica o ambiente profissional, incluindo trabalho e processos seletivos, como um dos principais locais percebidos de desigualdade.
- O teste Qui-Quadrado indicou associação estatisticamente significativa entre escolaridade e percepção dos locais de desigualdade.
- Também foram exploradas diferenças por renda, raça/cor, região e porte do município.

## Referências

- IPEC. Estudo 04839 - microdados utilizados na análise.
- IBGE. API SIDRA / Agregado 1378, Variável 93, usada para comparação demográfica.
- Documentação das bibliotecas Python utilizadas:
  - Pandas
  - Pyreadstat
  - Matplotlib
  - Seaborn
  - Plotly
  - SciPy
  - Requests