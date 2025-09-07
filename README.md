# Tweet Classification: Personal vs Non-Personal Health Mentions

## 📌 Overview
This project focuses on classifying tweets into two categories:
- **1 → Personal Health Mention**
- **0 → Non-Personal Health Mention**

The models are built using **sequence models (LSTM and Bi-LSTM)** with word embeddings to capture the semantic context of tweets. The task aims to explore how recurrent neural networks can effectively detect personal health mentions in short text.

---

## Dataset
- The dataset contains tweets labelled as:
  - `1` → Personal health mention
  - `0` → Non-personal health mention
- Tweets were preprocessed (tokenisation, stopword removal, padding) before training.

---

## Models Implemented
1. **LSTM (Long Short-Term Memory)**
   - Handles sequential dependencies in text.
   - Trained on tokenised and embedded tweets.

2. **Bi-LSTM (Bidirectional LSTM)**
   - Captures both past (backward) and future (forward) dependencies.
   - Expected to perform better than vanilla LSTM.

---

## Methodology
1. Data preprocessing (cleaning, tokenisation, padding).  
2. Embedding representation of words (e.g., Word2Vec, GloVe, or Keras Embedding Layer).  
3. Model building:
   - LSTM
   - Bi-LSTM
4. Hyperparameter tuning (dropout, learning rate, batch size, epochs).  
5. Model evaluation using accuracy, loss, and confusion matrix.  
6. Performance comparison.

---

## 📊 Results
| Model   | Accuracy | Loss  |
|---------|----------|-------|
| LSTM    | 83%      | 37%    |
| Bi-LSTM | 85%      | 34%   |

- Accuracy/loss curves included in the report.  
- Discussion of why Bi-LSTM outperformed or underperformed compared to LSTM.  

---


## 🚀 How to Run
```bash
# Clone repo
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook Tweet_Classification_LSTM_BiLSTM.ipynb
 
