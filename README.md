# spotify-data-project
# Análise de popularidade musical

Este projeto realiza uma análise de dados sobre as músicas mais populares do ano de 2023, utilizando informação da principal plataforma de streaming musical atualmente, o Spotify. O objetivo é identificar padrões e tendências nos gostos musicais dos ouvintes, focando em gêneros e período das faixas para validar ou não hipóteses.

## 📂 Dataset

O conjunto de dados utilizado é o `top_50_2023.csv`, importado da plataforma Kaggle, que contém informações detalhadas sobre cada faixa, incluindo:
* Nome do artista e da música
* Data de lançamento do álbum
* Gêneros musicais associados
* Características técnicas de áudio (dançabilidade, energia, etc.)
* Nível de popularidade

## 🎯 Hipóteses investigadas

A análise foi guiada pelas seguintes hipóteses:

1.  **H1:** O gênero 'Pop' é o mais predominante na lista, indicando ser o mais escutado pelos ouvintes.
2.  **H2:** As músicas de maior sucesso são lançamentos recentes, com a maioria datando de 2022 a 2023.

## 🛠️ Metodologia

O processo de análise foi estruturado da seguinte forma:

1.  **Carregamento e limpeza de Dados:**
    * Importação das bibliotecas necessárias (`pandas`, `seaborn`, `matplotlib`, `plotly`).
    * Leitura do arquivo `top_50_2023.csv`.
    * Renomeação de colunas para maior clareza (ex: `artist_name` para `artist`).
    * Conversão da duração das músicas de milissegundos para o formato `minutos:segundos`.

2.  **Engenharia de atributos:**
    * Criação da coluna `genero_simplificado` para agrupar subgêneros em categorias (Pop, Rap, R&B, Latin, Rock, Eletrônica e Outro).
    * Extração do ano de lançamento a partir da data completa para criar a coluna `ano_lancamento`.
    * Remoção de colunas com dados técnicos de áudio que não seriam utilizadas na análise principal.

3.  **Análise e visualização de Dados:**
    * Para a **H1**, foi gerado um gráfico de pizza para mostrar a distribuição percentual dos gêneros musicais simplificados.
    * Para a **H2**, foi criado um gráfico de barras para contar o número de músicas por ano de lançamento.

## 📈 Conclusões principais

A análise dos dados permitiu confirmar ambas as hipóteses:

* **Hipótese 1 (confirmada):** O gênero **Pop** é, de fato, o mais popular, representando **38%** das músicas na lista das 50 mais ouvidas, seguido por Rap e R&B.

* **Hipótese 2 (confirmada):** A grande maioria das músicas de sucesso são recentes. O gráfico de barras mostra a concentração de faixas lançadas em **2023** e **2022**, validando a ideia de que a popularidade está fortemente ligada a lançamentos novos.

## 🚀 Possíveis melhorias e autorreflexão

* **Análise de gêneros secundários:** A análise poderia ser aprofundada para verificar a influência de gêneros secundários (ex: músicas que são `Pop` mas também contêm `Rock` ou `Rap` em sua classificação).
* **Amostra maior:** Para obter insights mais robustos, a análise poderia ser replicada com um dataset maior (ex: Top 200) ou dados de outras plataformas musicais (Deezer, YouTube Music, etc.).

## 💻 Como executar o projeto

**1.** Você pode entrar na pasta do arquivo .ipynb incluído neste repositório.
**2.** Em seguida, já terá uma pré-visualização detalhada do projeto no próprio GitHub.
**3.** Além disso, pode clicar na opção "Open in Colab", que levará diretamente ao notebook do projeto no Google Colab.

1.  Clone este repositório:
    ```bash
    git clone
