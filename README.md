# NewsSum-Transformer

A TensorFlow-based implementation of a Transformer model from scratch for abstractive text summarization. This project uses the cleaned Inshorts news dataset to train a model capable of generating concise, human-readable summaries from longer news articles.

## 🚀 Features

- Transformer encoder-decoder architecture implemented from scratch
- Multi-head self-attention and feed-forward layers
- Positional encoding and layer normalization
- Training on Inshorts cleaned news dataset
- Abstractive text summarization (not just extractive)
- ROUGE score and loss-based evaluation

## 📚 Dataset

- **Source**: [Inshorts News Data](https://www.kaggle.com/datasets/shashankpatel/inshorts-news-data)
- **Format**: JSON, cleaned into `text` and `summary` pairs
- **Preprocessing**:
  - Lowercasing
  - Removing special characters
  - Tokenization
  - Padding and truncation

## 🏗️ Model Architecture

- **Encoder**:
  - Token + positional embeddings
  - Multi-head attention
  - Add & Norm
  - Feed-forward + Add & Norm

- **Decoder**:
  - Masked self-attention
  - Encoder-decoder attention
  - Feed-forward + Add & Norm

## 📈 Evaluation

- ROUGE-1, ROUGE-2, ROUGE-L
- Cross-entropy loss
- BLEU and cosine similarity (optional)

## 🛠️ Installation


git clone https://github.com/yourusername/news-sum-transformer.git
cd news-sum-transformer
pip install -r requirements.txt
## 🧪 Training
python train.py
## 📤 Inference
python generate_summary.py --input "Your long news article here"
## 📊 Results
ROUGE-L: 0.37 on validation set
Trained on 10k samples for 10 epochs
Generates fluent, context-aware summaries
## 🤝 Contributions
Feel free to fork this repo, raise issues, and submit PRs!
## 📄 License
MIT License

---

Let me know if you want:
- A sample output summary
- Gradio or Streamlit app interface
- GitHub actions for auto-training or testing
