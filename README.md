<div align="center">

# 📡 Árvore, Floresta ou Boosting?
### Previsão de Falha e Congestionamento em Enlaces de Rede com Machine Learning

[![Deploy Vercel](https://img.shields.io/badge/🌐_Site_No_Ar-Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://artigopreditorderedes.vercel.app/)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-159957?style=for-the-badge)](https://xgboost.readthedocs.io/)
[![Licença](https://img.shields.io/badge/Licença-CC_BY_4.0_%7C_MIT-2563eb?style=for-the-badge)](https://creativecommons.org/licenses/by/4.0/deed.pt_BR)

<p align="center">
  Artigo técnico e experimento prático comparando <strong>Árvore de Decisão</strong>, <strong>Random Forest (Bagging)</strong> e <strong>XGBoost (Boosting)</strong> no diagnóstico preditivo de quedas e degradação de redes.
</p>

<h3>
  👉 <a href="https://artigopreditorderedes.vercel.app/">Acesse o Artigo Interativo Publicado Aqui</a> 👈
</h3>

</div>

---

## 🎯 Sobre o Projeto## 👥 Autores * **Isaque Rodrigues Valim** | **Eduardo Felipe** | **Ryan Catão de Paula** | **Gabriel José Couto Pereira** | **Gabriel Schmidit]**

Links de rede raramente caem sem aviso prévio. Antes de uma interrupção severa, métricas de telemetria dão sinais claros de degradação. Este projeto investiga qual arquitetura baseada em árvores oferece o melhor equilíbrio entre **capacidade de detecção (Recall/F1-Score)**, **custo operacional de erros (Falsos Negativos vs. Falsos Positivos)**, **latência de inferência** e **interpretabilidade**.

### 📊 Os Três Modelos Avaliados
1. **🌳 Árvore de Decisão (*Decision Tree*):** Modelo base estruturado em cortes sucessivos de pureza (Gini/Entropia), com controle de *overfitting* via poda (`max_depth`).
2. **🌲 Random Forest (*Bagging*):** Conjunto (*ensemble*) de árvores independentes treinadas em paralelo com amostragem *bootstrap* e votação majoritária para **redução de variância**.
3. **🚀 XGBoost (*Extreme Gradient Boosting*):** Conjunto de árvores treinadas de forma sequencial, onde cada nova árvore corrige os erros residuais da anterior orientadas pelo gradiente, com regularização nativa para **redução de viés**.

---

## 🗂️ Estrutura do Repositório

```text
📦 Artigo_Preditor_de_redes/
 ┣ 📂 Notebooks_Testes/          # Scripts e Notebooks Jupyter com os experimentos e métricas
 ┣ 📂 Website/                   # Código-fonte da página publicada na Vercel
 ┃ ┣ 📂 css/
 ┃ ┃ ┗ 📜 style.css              # Estilização responsiva (Dark Mode Tech)
 ┃ ┣ 📂 img/                     # Fotografias dos autores e recursos gráficos
 ┃ ┗ 📜 index.html               # Artigo completo, diagramas SVG e tabelas comparativas
 ┣ 📜 README.md                  # Documentação e guia de reprodutibilidade
 ┗ 📜 requirements.txt           # Dependências exatas do ambiente Python

## 🗂️ Como rodar o projeto:
->O código deve ser inserido na pasta "my_drive" disponível em todo google drive.
->A permissão para acesso do Google Drive deve ser concedido ao aplicativo google colab
-> O notebook deve ser upado nele (Google Colab) e executado bloco a bloco
