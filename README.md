# 🎵 Projeto ETL - Biblioteca de Músicas

Este projeto realiza um pipeline ETL (Extração, Transformação e Carregamento) sobre uma coleção de músicas de diferentes artistas e estilos, com o objetivo de gerar insights a partir das informações.

🎧 A seleção das músicas foi feita manualmente por mim, com base em preferências pessoais e interesse em analisar diferentes gêneros, artistas e níveis de popularidade.

## 🗂️ Estrutura do projeto

- 📁 `data/musicas.csv`: arquivo original com dados das músicas.
- 📓 `notebooks/musica_etl_pipeline.ipynb`: notebook com o pipeline ETL, transformações e análises.
- 📄 `output/musicas_tratadas.csv`: arquivo CSV gerado após as transformações.
- 🖼️ `prints/` – capturas de tela com os resultados dos códigos e visualizações.
  
## ⚙️ Pipeline ETL

### 📂 Extração (Extract)
- Leitura dos dados a partir do CSV original.

### ✏️ Transformação (Transform)
- Padronização dos nomes das colunas.
- Conversão da duração de segundos para minutos.
- Formatação das visualizações em milhões (M) e bilhões (B).
- Consultas como top 10 músicas mais visualizadas e contagem por gênero.

### 🔄 Carregamento (Load)
- Salvamento do arquivo tratado em CSV para uso posterior.

## 🔍 Principais Insights

- 🎶 **Música mais visualizada**: A música mais visualizada da lista é **"Rolling in the Deep"** da **Adele**, com **2.6 bilhões** de visualizações no YouTube — destacando seu enorme impacto global.  
- 📈 **Ano com maior número de músicas**: O ano com maior número de músicas listadas é **2003**, com destaque para o gênero **Rock** — refletindo um período marcante para esse estilo musical.  
- 🌍 **Gênero musical predominante**: O gênero musical mais frequente no dataset é o **Rock**, seguido por **Pop** e **R&B** — mostrando a preferência e popularidade desses estilos no conjunto analisado.  
- ⏱️ **Duração média das músicas**: A média de duração das músicas é de aproximadamente **3,9 minutos**, sendo a mais longa **"Here Without You"** com **4,25 minutos** — indicando uma variação típica para canções populares.  
- 📺 **Visualizações totais no YouTube**: As músicas listadas somam mais de **15 bilhões** de visualizações combinadas no YouTube — evidenciando o alcance e a relevância das faixas selecionadas.  
- 🎧 **Diversidade de gêneros**: Há diversidade de gêneros, com presença de **Nu Metal**, **Rock Alternativo** e **Pop Rock** — refletindo diferentes épocas e estilos musicais no dataset.  
- 👤 **Escolha pessoal e curadoria manual**: A seleção de músicas foi feita manualmente, baseada em preferências pessoais e no impacto cultural e comercial das faixas — garantindo diversidade e representatividade na base.  


## 📊 Exemplos Visuais

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


