# 🎵 Projeto ETL - Biblioteca de Músicas

Este projeto realiza um pipeline ETL (Extração, Transformação e Carregamento) sobre uma coleção de músicas de diferentes artistas e estilos, com o objetivo de gerar insights a partir das informações.

🎧 A seleção das músicas foi feita manualmente por mim, com base em preferências pessoais e interesse em analisar diferentes gêneros, artistas e níveis de popularidade.

- ## 📁 Estrutura do Projeto

- 📁 `data/musicas.csv`: arquivo original com dados das músicas.
- 📓 `notebooks/musica_etl_pipeline.ipynb`: notebook com o pipeline ETL, transformações e análises.
- 📄 `output/musicas_tratadas.csv`: arquivo CSV gerado após as transformações.
- 🖼️ `prints/`: capturas de tela com os resultados dos códigos e visualizações.
- 🧠 `analises/insights.md`: arquivo contendo os principais insights obtidos a partir da análise dos dados.
  
## ⚙️ Pipeline ETL

### 📂 Extração (Extract)
- Leitura dos dados a partir do CSV original.

### ✏️ Transformação (Transform)
- Padronização dos nomes das colunas.
- Conversão da duração de segundos para minutos.
- Formatação das visualizações em milhões (M) e bilhões (B).

### 🧠 Análise (Analyze)
- Consultas como top 10 músicas mais visualizadas e contagem por gênero.
- Geração de insights a partir das transformações e estatísticas exploratórias.
- Interpretação dos padrões encontrados (duração média, gêneros predominantes, ano com mais músicas, etc.).
- Resultados documentados no arquivo `analises/INSIGHTS.md`.

### 🔄 Carregamento (Load)
- Salvamento do arquivo tratado em CSV para uso posterior.

## ⚙️ Principais Funções do Pipeline ETL

- `carregar_dados(caminho)`: lê o arquivo CSV original e retorna o DataFrame com os dados das músicas.
- `padronizar_colunas(df)`: padroniza os nomes das colunas para minúsculas e sem espaços.
- `converter_duracao(df)`: converte a duração das músicas de segundos para minutos, criando uma nova coluna e removendo a original.
- `formatar_visualizacoes(x)`: função auxiliar que formata números de visualizações em milhões (M) e bilhões (B).
- `adicionar_visualizacoes_formatadas(df)`: aplica a formatação de visualizações e adiciona uma nova coluna ao DataFrame.
- `ordenar_por_visualizacoes(df)`: ordena o DataFrame com base no número de visualizações, do maior para o menor.
- `plotar_top_10_visualizacoes(df)`: gera um gráfico de barras com as 10 músicas mais visualizadas.
- `filtrar_por_genero(df, genero)`: retorna as músicas filtradas por gênero musical.
- `contar_musicas_por_ano(df)`: retorna a contagem de músicas por ano de lançamento.
- `contar_musicas_por_genero(df)`: retorna a contagem de músicas por gênero.
- `salvar_csv(df, caminho_saida)`: salva o DataFrame transformado em um arquivo CSV.

## 💡 Insights

Os principais achados da análise exploratória estão no arquivo [`analises/insights.md`](analises/insights.md).

## 📷 Exemplos Visuais

### Top 10 músicas mais visualizadas
![Top 10 músicas mais visualizadas - Código](prints/top_10_visualizacoes_1.png)

![Top 10 músicas mais visualizadas - Gráfico](prints/top_10_visualizacoes_2.png)

### Filtro simples de gênero
![Distribuição por gênero](prints/filtro_genero.png)

### Contagem de músicas por gênero
![Contagem por gênero](prints/contagem_genero.png)

### Distribuição por ano de lançamento
![Distribuição ano de lançamento](prints/distribuicao_ano_lancamento.png)

## 📦 Requisitos

- Python 3.x
- Jupyter Notebook
- Bibliotecas: pandas, matplotlib, seaborn

## ▶️ Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seuusuario/musicas-etl.git
   cd musicas-etl

2. (Opcional) Crie um ambiente virtual:
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows

3. Instale as dependências:
pip install -r requirements.txt

4. Execute o notebook:
jupyter notebook notebooks/musica_etl_pipeline.ipynb

---
✍️ Autor: Lidiane  
🏠 GitHub: [LidianeSouza](https://github.com/LidianeSouza)
📅 Projeto desenvolvido como parte do desafio DIO

📄 Licença: MIT


