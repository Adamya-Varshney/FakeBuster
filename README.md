# 🕵️‍♂️ FakeBuster: Detect & Explain Fake News and Deepfakes using GenAI

**FakeBuster** is a multimodal Generative AI system designed to detect, explain, and mitigate the spread of **fake news** and **deepfakes** across **text, image, and video** content. It combines state-of-the-art models in GenAI with RAG, embeddings, and explainability features to enable **real-time content verification**—especially useful during elections, disasters, conflicts, or pandemics.

---

## 🚀 Features

- ✅ **Multimodal Input**: Analyze content from tweets, news snippets, images, and video clips.
- ✅ **AI-Generated Content Detection**: Classify content as real, fake, or AI-generated.
- ✅ **Explainability**: Generate natural language justifications for each classification.
- ✅ **Fact Verification**: Suggest reliable sources using RAG (Retrieval-Augmented Generation).
- ✅ **Structured Output**: JSON-formatted results for easy API integration.
- ✅ **Vector Search**: Uses embeddings to match with verified knowledge base.
- ✅ **GenAI Evaluation**: Evaluate model output quality across modalities.

---

## 🧠 Tech Stack

- **LLMs**: OpenAI GPT / LLaMA 2 / Mistral (Configurable)
- **Embeddings**: OpenAI / HuggingFace Transformers
- **RAG**: LangChain / Haystack
- **UI**: Streamlit / Gradio (Coming Soon)
- **Backend**: Python, FastAPI (optional)
- **Databases**: FAISS, Pinecone (for vector search)

---

## 📂 Datasets Used

| Dataset | Description |
|---------|-------------|
| [Misinformation Graph](https://www.kaggle.com/datasets/arashnic/misinfo-graph) | Graph-based data for fake/real text classification |
| [FakeNewsNet](https://www.kaggle.com/datasets/mdepak/fakenewsnet) | Real-world news articles labeled real/fake |
| [Deepfake Detection Challenge](https://www.kaggle.com/c/deepfake-detection-challenge) | Video clips for deepfake detection |

---

## 📁 Project Structure
---

## 🧪 How to Run

### 1. Clone the repository

git clone https://github.com/yourusername/FakeBuster.git
cd FakeBuster

### 2. Install Dependencies
pip install -r requirements.txt

### 3. Run Inference
python src/main.py --input "sample_tweet.txt" --type text

📌 Use Cases
- Social media moderation

- Fact-checking in journalism

- Real-time browser plugin for misinformation detection

- Media literacy tools

🛣️ Roadmap
 - Text fake news detection + explainability

 - Image deepfake detection

 - Video deepfake classification

 - Web UI (Streamlit)

 - API Integration (FastAPI)

 - Evaluation Dashboard

🤝 Contributing
Contributions are welcome!

- Fork the repo

- Create your branch: feature/your-feature-name

- Commit your changes

- Open a Pull Request

📜 License
This project is currently unlicensed. Contact the maintainer for permissions regarding reuse.

👨‍💻 Maintainer

Email: adamya1998official@gmail.com |noel | Himanshi

⭐ If you find this useful, give it a star and share it with others!
