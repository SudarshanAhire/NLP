# Game of Thrones Word2Vec Analysis

A Natural Language Processing (NLP) project that trains a **Word2Vec model** on the *Game of Thrones* book dataset to learn semantic relationships between characters, locations, and important terms from the series.

---

# 📌 Project Overview

This project uses the **Word2Vec algorithm** from the `gensim` library to analyze text data from the *Game of Thrones* books.

The model learns contextual meaning of words and can:

- Find similar characters or words
- Measure similarity between characters
- Detect odd words from a list
- Generate vector embeddings
- Visualize embeddings in 3D space

---

# 🚀 Technologies Used

- Python
- NumPy
- Pandas
- Gensim
- NLTK
- Scikit-learn
- Plotly
- KaggleHub
- Jupyter Notebook

---

# 📂 Dataset

Dataset: **Game of Thrones Books Dataset**

Source: Kaggle

The dataset is downloaded dynamically using:

```python
import kagglehub 


⚙️ Features
✅ Text Preprocessing
Sentence tokenization
Word tokenization
Lowercase conversion
Stopword handling
Text cleaning using simple_preprocess


✅ Word2Vec Model Training

The project trains a custom Word2Vec model using:

Word2Vec(sentences=processed_sentences,
         vector_size=100,
         window=5,
         min_count=2,
         workers=4)


✅ NLP Operations
Find Similar Words
model.wv.most_similar('daenerys')

Check Similarity Between Words
model.wv.similarity('arya', 'sansa')

Detect Odd Word
model.wv.doesnt_match(['jon', 'arya', 'bran', 'dragon'])

Access Word Vectors
model.wv['jon']


📊 Visualization

The project uses:

PCA (Principal Component Analysis)
Plotly 3D Scatter Plot

to visualize high-dimensional word embeddings in 3D space.

This helps understand semantic clustering of characters and terms.



🛠️ Installation
Clone Repository
git clone https://github.com/your-username/game-of-thrones-word2vec.git
Install Dependencies
pip install numpy pandas gensim nltk scikit-learn plotly kagglehub


▶️ Run the Project

Start Jupyter Notebook:

jupyter notebook

Open:

game_of_thrones_word2vec.ipynb

Run all cells to train the model and visualize embeddings.


📈 Output Examples
Similarity scores between characters
Word relationship analysis
Semantic clustering visualization
Interactive 3D embedding graph



📚 Learning Outcomes

This project helps understand:

Natural Language Processing (NLP)
Word Embeddings
Word2Vec Algorithm
Text preprocessing techniques
Semantic similarity
Dimensionality reduction using PCA
Data visualization



🔮 Future Improvements
Add TSNE visualization
Use larger fantasy datasets
Build character relationship networks
Create a web application
Add sentiment analysis


👨‍💻 Author

Sudarshan Ahire


⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.