# 🎧 Spotify Music Recommender System  
Pipeline Completo (ETL + Machine Learning + Visualizações Estilo Spotify)

Este repositório apresenta um projeto completo envolvendo engenharia de dados, ciência de dados e machine learning, construído em Databricks + Apache Spark, com o objetivo de:

- Criar um ETL robusto para tratar uma base de músicas
- Preparar dados para análise e modelagem
- Implementar um sistema de recomendação musical
- Reduzir dimensionalidade com PCA
- Agrupar músicas com KMeans
- Gerar visualizações profissionais, incluindo exibição de capas estilo Spotify

---

## 📂 Estrutura do Repositório

```
.
├── notebooks/
│   ├── SPOTIFY_ETL.py
│   ├── RECOMENDADOR_SPOTIFY.py
│
├── images/
└── README.md
```

---

## 🚀 Visão Geral do Projeto

### 🧱 1. ETL — Engenharia de Dados com Spark

O notebook `SPOTIFY_ETL.py` realiza:

- Ingestão da base de músicas
- Padronização das colunas
- Conversão segura de tipos usando try_cast
- Feature Engineering das variáveis musicais
- Salvamento otimizado em Parquet

### 🔮 2. PCA + KMeans — Clusterização Musical

O notebook `RECOMENDADOR_SPOTIFY.py` realiza:

- Redução de dimensionalidade com PCA (2D/3D)
- Agrupamento de músicas com KMeans
- Análises temporais e exploração de variáveis
- Scatter interativo Plotly
- Similaridade no espaço PCA

### 🎵 3. Sistema de Recomendação

- Identifica cluster da música selecionada
- Filtra músicas do mesmo cluster
- Calcula distância euclidiana no espaço PCA
- Ordena pelas mais semelhantes
- Retorna Top-N recomendações

---

## 🖼 4. Visualizações Estilo Spotify

O projeto inclui:

- Grid de capas com cantos arredondados
- Layout escuro tipo Spotify (#121212)
- Visualização interativa com Plotly
- Gráficos temporais e analíticos
- PCA com hover mostrando artista/música

---

## 🛠 Tecnologias Utilizadas

- Databricks  
- Apache Spark (PySpark)  
- PCA, KMeans (Scikit-Learn)  
- Plotly, Matplotlib  
- Pillow (PIL)  
- Spotipy (opcional)

---

## 📁 Como Executar

```
git clone https://github.com/uiliannunes/spotify_recomendation.git
cd spotify-recommender
pip install -r requirements.txt
```

Execute os notebooks em Databricks, Colab, VSCode ou Jupyter.

---

## 🔑 API do Spotify (Opcional)

Crie chaves em:

https://developer.spotify.com/dashboard

Configuração:

```python
client_id = "SEU_CLIENT_ID"
client_secret = "SEU_CLIENT_SECRET"
redirect_uri = "http://localhost:8888/callback"
```

---

## 🧠 Resultados

- Recomendações musicais precisas  
- Clusters bem definidos  
- PCA interativo  
- Visual profissional de capas  
- Pipeline ETL preparado para produção  

---

## 📬 Contato

- LinkedIn: https://linkedin.com/in/uiliannunes  
- GitHub: https://github.com/uiliannunes

---

## 📄 Licença

MIT License
