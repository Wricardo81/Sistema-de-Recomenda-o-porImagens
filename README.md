# 🔍 Sistema de Recomendação por Similaridade de Imagens

Este projeto tem como objetivo desenvolver um sistema inteligente capaz de recomendar produtos similares com base 
em suas **características visuais** — como cor, forma, textura — ao invés de atributos textuais como nome, marca ou preço.  

🧠 Baseado em técnicas de **Deep Learning**, utilizando redes convolucionais (CNNs) para extração de características
de imagens e algoritmos de vizinhança para recomendação.

---

## 📌 Funcionalidades

- Extração de **vetores de características** (embeddings) de imagens usando modelos pré-treinados.
- Cálculo de similaridade visual entre imagens.
- Retorno dos **k produtos mais semelhantes visualmente** a uma imagem de entrada.
- Possibilidade de uso via **interface interativa** (Gradio/Streamlit - opcional).
- Suporte a diversas classes de produtos (roupas, relógios, calçados, bicicletas, etc).

---

## 📁 Estrutura do Projeto

```bash
image-similarity-recommender/
│
├── data/                  # Imagens organizadas por categoria
│   ├── camisa/
│   ├── relogio/
│   └── sapato/
│
├── embeddings/            # Vetores extraídos das imagens
├── notebooks/
│   └── image_similarity.ipynb  # Notebook principal
│
├── app/                   # Interface (opcional)
│   └── interface.py
│
├── utils/
│   └── extractor.py       # Código para extrair features
│   └── recommender.py     # Código para recomendação
│
├── requirements.txt
└── README.md


🚀 Como Executar
1. Clone o repositório
bash
Copiar
Editar
git clone https://github.com/seu-usuario/image-similarity-recommender.git
cd image-similarity-recommender
2. Crie um ambiente virtual e instale as dependências
bash
Copiar
Editar
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

pip install -r requirements.txt
3. Organize as imagens
Crie pastas dentro da pasta data/ separando os produtos por classe (ex: camisa, relogio, sapato, etc).

4. Execute o notebook principal
No Colab ou localmente:

bash
Copiar
Editar
jupyter notebook notebooks/image_similarity.ipynb
🛠 Tecnologias Utilizadas
Python

TensorFlow / Keras

NumPy, Matplotlib, Scikit-learn

FAISS (Facebook AI Similarity Search) [opcional]

Gradio / Streamlit (para interface)

Google Colab (para execução rápida)

📷 Exemplos de Recomendação
Imagem consultada:

<p align="center"><img src="exemplo/input.jpg" width="200"/></p>
Resultados recomendados:

<p align="center"> <img src="exemplo/rec1.jpg" width="150"/> <img src="exemplo/rec2.jpg" width="150"/> <img src="exemplo/rec3.jpg" width="150"/> </p>
