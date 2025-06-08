# 🎵 Projeto ETL - Biblioteca de Músicas

Este projeto realiza um pipeline ETL (Extração, Transformação e Carga) sobre uma coleção de músicas de diferentes artistas e estilos, com o objetivo de gerar insights a partir das informações.

## 🗂️ Estrutura do projeto

- 📁 `data/musicas.csv`: arquivo original com dados das músicas.
- 📓 `notebooks/musica_etl_pipeline.ipynb`: notebook com o pipeline ETL, transformações e análises.
- 📄 `output/musicas_tratadas.csv`: arquivo CSV gerado após as transformações.
- 🖼️ `prints/´ – capturas de tela com os resultados e gráficos
  
## 🔄 Pipeline ETL

- 📥 **Extração (Extract)**: dados em CSV com colunas como título, artista, gênero e avaliação
- 🔧 **Transformação (Transform)**: limpeza, análise e enriquecimento dos dados
- 📤 **Carregamento (Load)**: exportação para novo CSV ou visualização interativa

## 📊 Visualizações

### Top 10 músicas mais visualizadas
![Top 10 músicas mais visualizadas - Código](prints/top_10_visualizacoes_1.png)

![Top 10 músicas mais visualizadas - Gráfico](prints/top_10_visualizacoes_2.png)

### Filtro simples de gênero
![Distribuição por gênero](prints/filtro_genero.png)

### Contagem de músicas por gênero
![Contagem por gênero](prints/contagem_genero.png)

### Distribuição por ano de lançamento
![Distribuição ano de lançamento](prints/distribuicao_ano_lancamento.png)

## ▶️ Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seuusuario/musicas-etl.git
   cd musicas-etl
