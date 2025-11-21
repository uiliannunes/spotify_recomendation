# 🎧 Spotify Music Recommender System  
*Um projeto completo usando Databricks, Spark, PCA, KMeans e API do Spotify*

Este repositório contém dois notebooks que, juntos, formam um pipeline completo de recomendação musical usando dados do Spotify.  
O projeto inclui:

- Extração de dados reais via **API do Spotify**  
- Limpeza e padronização com **PySpark**  
- Feature Engineering de áudio (energy, danceability, valence, etc.)  
- Redução de dimensionalidade com **PCA**  
- Clusterização com **KMeans**  
- Visualizações avançadas usando **Plotly**  
- Exibição de capas das músicas com visual estilo Spotify  
- Sistema de recomendação baseado em vizinhança no espaço PCA  

---

## 📂 Estrutura do Repositório

```
.
├── notebooks/
│   ├── spotify_etl_artists_pipeline.ipynb
│   ├── recomendador_spotify.ipynb
│
├── images/
└── README.md
```

---

## 🚀 Tecnologias Utilizadas

### Backend / Pipeline
- Databricks  
- Apache Spark  
- PySpark  
- Spotipy (API do Spotify)

### Machine Learning
- PCA  
- KMeans  
- scikit-learn

### Visualizações
- Plotly  
- Matplotlib  
- PIL (Pillow)

---

## 🎵 O que o Projeto Faz?

### ✔️ ETL de dados do Spotify
- Pipeline Spark
- Conversão de tipos
- Salvamento em Parquet

### ✔️ Feature Engineering
- Tratamento de colunas
- Conversões com try_cast
- Padronização de dados musicais

### ✔️ Clusterização
- Agrupamento de músicas com KMeans

### ✔️ Redução com PCA
- Projeção 2D/3D  
- Visualização interativa

### ✔️ Recomendador
- Similaridade no espaço PCA  
- Filtro por cluster  
- Ranking por proximidade

### ✔️ Grid de capas estilo Spotify
- Cantos arredondados  
- Fundos escuros  
- Visual premium  

---

## 📁 Como Executar

```
git clone https://github.com/uiliannunes/spotify_recomendation.git
cd spotify-recommender
pip install -r requirements.txt
```

Abra os notebooks em Databricks, Jupyter ou VSCode.

---

## 🔑 Configuração da API do Spotify

Crie chaves em:  
👉 https://developer.spotify.com/dashboard

Configure:

```python
client_id = "SEU_CLIENT_ID"
client_secret = "SEU_CLIENT_SECRET"
redirect_uri = "http://localhost:8888/callback"
```

---

## 🧠 Resultados

- Sistema recomendador funcional  
- Clusters coerentes  
- PCA interativo  
- Visual profissional de capas  

---

## 📬 Contato

- LinkedIn: https://linkedin.com/in/uiliannunes  
- GitHub: https://github.com/uiliannunes  

---

## 📄 Licença

MIT License
