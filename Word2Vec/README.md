# ⚔️ Game of Thrones Word2Vec

A Natural Language Processing (NLP) project that implements the **Word2Vec** algorithm using the **Game of Thrones books dataset**.  
This project learns semantic relationships between characters, places, and important words from the series using word embeddings.

---

# 📌 Project Overview

This project demonstrates how Word2Vec converts words into meaningful numerical vectors based on their surrounding context in text data.

Using the trained model, we can:

- Find similar characters or words
- Measure similarity between characters
- Detect unrelated words
- Extract word embeddings
- Visualize high-dimensional vectors in 3D space

---

# 🚀 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Gensim | Word2Vec Implementation |
| NLTK | Text Preprocessing |
| NumPy | Numerical Operations |
| Pandas | Data Handling |
| Scikit-learn | PCA Dimensionality Reduction |
| Plotly | 3D Visualization |
| KaggleHub | Dataset Download |

---

# 📂 Dataset

Dataset Used:

**Game of Thrones Books Dataset**

The dataset is downloaded directly using KaggleHub.

---

# ⚙️ Workflow

## 1️⃣ Dataset Loading

The Game of Thrones dataset is downloaded and loaded into the notebook.

```python
import kagglehub

data = kagglehub.dataset_download("khulasasndh/game-of-thrones-books")
```

---

## 2️⃣ Text Preprocessing

The text data is preprocessed using:

- Sentence Tokenization
- Word Tokenization
- Lowercase Conversion
- Text Cleaning
- Stopword Handling
- `simple_preprocess()` from Gensim

---

## 3️⃣ Word2Vec Model Training

The Word2Vec model is trained using:

```python
model = gensim.models.Word2Vec(
    window=10,
    min_count=2
)
```

Vocabulary is built and the model is trained on the processed text.

---

## 4️⃣ NLP Operations

### ✅ Find Similar Words

```python
model.wv.most_similar('daenerys')
```

---

### ✅ Detect Odd Word

```python
model.wv.doesnt_match(['jon','rikon','robb','arya','sansa','bran'])
```

---

### ✅ Calculate Similarity

```python
model.wv.similarity('arya','sansa')
```

---

### ✅ Access Word Vectors

```python
model.wv['king']
```

---

# 📊 Visualization

The project uses:

- PCA (Principal Component Analysis)
- Plotly 3D Scatter Plot

to visualize Word2Vec embeddings in 3D space.

```python
fig = px.scatter_3d(
    X[200:300],
    x=0,
    y=1,
    z=2,
    color=y[200:300]
)
```

This helps understand semantic clustering between related words.

---

# 🛠️ Installation

## Clone Repository

```bash
git clone https://github.com/SudarshanAhire/NLP.git
```

---

## Move to Project Folder

```bash
cd NLP/Word2Vec
```

---

## Install Dependencies

```bash
pip install numpy pandas gensim nltk scikit-learn plotly kagglehub
```

---

# ▶️ Run the Project

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```bash
game_of_thrones_word2vec.ipynb
```

Run all notebook cells sequentially.

---

# 📚 Concepts Covered

- Natural Language Processing (NLP)
- Text Preprocessing
- Word Embeddings
- Word2Vec
- Semantic Similarity
- Vector Representation
- PCA
- Data Visualization

---

# 🔮 Future Improvements

- Add TSNE visualization
- Compare CBOW and Skip-Gram
- Add FastText implementation
- Train on larger datasets
- Build interactive NLP visualization dashboard

---

# 📁 Project Structure

```bash
Word2Vec/
│
├── game_of_thrones_word2vec.ipynb
├── README.md
└── dataset/
```

---

# 👨‍💻 Author

## Sudarshan Ahire

Computer Engineering Student | AI/ML & NLP Enthusiast

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.