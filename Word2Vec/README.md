# Word2Vec using Game of Thrones Dataset ⚔️

This project demonstrates the implementation of the **Word2Vec** algorithm using text data from the **Game of Thrones** book series.  
The model learns semantic relationships between words, characters, and locations by analyzing the context in which words appear.

The project also includes preprocessing, similarity analysis, vector extraction, and 3D visualization of word embeddings.

---

# 📌 Project Objective

The main objective of this project is to understand how **Word Embeddings** work in Natural Language Processing (NLP).

Using Word2Vec, the model can:

- Learn relationships between words
- Identify similar characters
- Measure semantic similarity
- Detect unrelated words
- Convert words into dense numerical vectors
- Visualize embeddings in 3D space

---

# 🚀 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Gensim | Word2Vec Model |
| NLTK | Text Processing |
| Pandas | Data Handling |
| NumPy | Numerical Operations |
| Scikit-learn | PCA Dimensionality Reduction |
| Plotly | Interactive Visualization |
| KaggleHub | Dataset Downloading |
| Jupyter Notebook | Development Environment |

---

# 📂 Dataset

Dataset Used:  
**Game of Thrones Books Dataset**

The dataset contains textual content from the Game of Thrones novels.

---

# ⚙️ Workflow

## 1️⃣ Data Collection
- Dataset downloaded using KaggleHub

## 2️⃣ Text Preprocessing
The text is cleaned and processed using:
- Sentence tokenization
- Word tokenization
- Lowercase conversion
- Removal of unwanted symbols
- Stopword handling
- `simple_preprocess()` from Gensim

## 3️⃣ Model Training
A custom Word2Vec model is trained on the processed text data.

## 4️⃣ Word Analysis
The trained model is used for:
- Similar word detection
- Word similarity checking
- Odd-word identification
- Word vector extraction

## 5️⃣ Visualization
High-dimensional vectors are reduced to 3D using PCA and visualized using Plotly.

---

# 🧠 Word2Vec Concepts Used

## ✅ CBOW (Continuous Bag of Words)
Predicts a target word using surrounding context words.

## ✅ Skip-Gram
Predicts surrounding words using a target word.

## ✅ Word Embeddings
Converts words into meaningful dense vectors.

---

# 📊 Example Operations

## Find Similar Words

```python
model.wv.most_similar('daenerys')
```

---

## Calculate Similarity Between Characters

```python
model.wv.similarity('arya', 'sansa')
```

---

## Find Odd Word

```python
model.wv.doesnt_match(['jon', 'arya', 'bran', 'dragon'])
```

---

## Access Word Vector

```python
model.wv['jon']
```

---

# 📈 Visualization

The project visualizes word embeddings using:

- PCA (Principal Component Analysis)
- Plotly 3D Scatter Plot

This helps in understanding how semantically related words cluster together.

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
pip install numpy pandas nltk gensim scikit-learn plotly kagglehub
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

Run all cells sequentially.

---

# 📚 Learning Outcomes

After completing this project, you will understand:

- NLP preprocessing pipeline
- Word2Vec algorithm
- Word embeddings
- Semantic similarity
- Vector representation of text
- PCA dimensionality reduction
- NLP visualization techniques

---

# 🔮 Future Improvements

- Add TSNE visualization
- Train on larger NLP datasets
- Add FastText implementation
- Add Glove embeddings
- Create a web-based NLP visualizer
- Compare CBOW vs Skip-Gram performance

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

Computer Engineering Student | AI/ML Enthusiast | NLP Learner

---

# ⭐ Support

If you found this project useful, consider giving this repository a ⭐ on GitHub.