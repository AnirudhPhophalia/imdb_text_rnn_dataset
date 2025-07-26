# 🎮 Sentiment Analysis with LSTM (IMDb Movie Reviews)

This project uses a **Recurrent Neural Network (RNN)** with **LSTM layers** to classify IMDb movie reviews as either **positive** or **negative**. The model is trained and evaluated on the built-in IMDb dataset available in TensorFlow.

---

## 📊 Model Performance

* **Test Accuracy**: 82%
* **Precision (Positive class)**: 80%
* **Recall (Positive class)**: 86%
* **F1-Score**: 0.83

📌 **Confusion Matrix**:

```
                Predicted
              ┌───────────────────────────────┌
              │   0   │   1   │
┌───────────────────────────────├
│ Actual  0   │ 9878  │ 2622  │
│ Actual  1   │ 1811  │ 10689 │
└───────────────────────────────┘
```

---

## 📁 Dataset

* **Source**: [IMDb reviews](https://www.tensorflow.org/datasets/catalog/imdb_reviews)
* **Total Samples**: 50,000

  * 25,000 for training
  * 25,000 for testing
* **Labels**: Binary (0 = Negative, 1 = Positive)

---

## 🧠 Model Architecture

* `Embedding` Layer (vocab\_size = 10,000, embedding\_dim = 64)
* `Bidirectional LSTM` Layer 1: 64 units (return\_sequences=True)
* `Bidirectional LSTM` Layer 2: 32 units
* `Dropout`: 0.5
* `Dense` Output Layer with `Sigmoid` activation

---

## 📦 Requirements

Install the following before running:

```bash
pip install tensorflow matplotlib scikit-learn
```

---

## 🚀 How to Run

1. Open in Google Colab or Jupyter Notebook
2. Copy and paste the code from `main.ipynb`
3. Train the model
4. Evaluate accuracy
5. Use your own reviews to test predictions

---

## ✨ Future Improvements

* Use custom real-text datasets (.csv)
* Add an option to predict our own reviews
* Try GRU or Transformer-based models (e.g., BERT)
* Deploy using Streamlit or Flask
* Add attention mechanism

---

## 🧑‍💻 Author

**Anirudh Phophalia**
*This project is built for learning deep learning with text (NLP) using RNN architectures.*
