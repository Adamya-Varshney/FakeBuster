# 🧠 FakeBuster – Get Your Facts Right

**FakeBuster** is an LLM-powered interactive system built to **detect hallucinations**, **evaluate groundedness**, and **critique factual correctness** in generated responses. It combines **retrieval-augmented generation (RAG)**, **Google’s Gemini Pro**, and **LangChain** to verify answers against trusted documents and highlight unsupported claims.

---

## 🚀 Features

- ✅ **Question Answering Agent**: Powered by Gemini Pro with tool integration for document-grounded QA.
- ✅ **Document Embedding**: Uses `GoogleGenerativeAIEmbeddings` to semantically index knowledge.
- ✅ **Chunking + Retrieval**: Documents are split and retrieved using `RecursiveCharacterTextSplitter`.
- ✅ **Fact Verification**: Responses are cross-checked against source chunks with contextual prompts.
- ✅ **Factual Consistency Critique**: Detects hallucinations using structured evaluation prompts.
- ✅ **Evaluation Reports**: Outputs structured JSON/Pandas reports for each response.
- ✅ **Optional HuggingFace Evaluation**: Supports additional model-based critiques via `InferenceClient`.

---

## 🧰 Tech Stack

- **LLM**: Gemini Pro (`ChatGoogleGenerativeAI`)
- **Embeddings**: Google Generative AI Embedding Model
- **RAG Framework**: LangChain
- **Vector Store**: ChromaDB (configurable)
- **Visualization**: Pandas, IPython Display
- **Tools**: LangChain Agent with custom Tools + HuggingFace Hub integration

---

## ⚙️ Setup

Install required packages:

```bash
pip install -U langchain chromadb google-generativeai huggingface_hub tqdm pandas datasets
```
## 📁 Functional Highlights

| Component                         | Role                                           |
|----------------------------------|------------------------------------------------|
| `GoogleGenerativeAIEmbeddings`   | Convert chunks into embedding vectors          |
| `ChatGoogleGenerativeAI`         | Answer questions using Gemini Pro              |
| `RecursiveCharacterTextSplitter` | Chunk source docs for dense retrieval          |
| `Tool Agent + reset_tool_usage()`| Orchestrate retrieval & critique               |
| `evaluation.load_evaluator()`    | Score responses for factuality & grounding     |
| `InferenceClient` (optional)     | Classify hallucination likelihood              |


## 🧪 Workflow

1. **Load documents** and split into chunks.
2. **Embed chunks** and index into a vector store.
3. **Accept a query** → retrieve top-k chunks using cosine similarity.
4. **Generate an answer** via Gemini Pro based on retrieved evidence.
5. **Critique** the generated answer using a structured prompt.
6. **Display hallucination detection** and retrieval fidelity results.


## 🔐 Environment Variables

To run this project, set the following environment variables:

```bash
export GOOGLE_API_KEY=your_google_key
export OPENAI_API_KEY=your_openai_key
```
```bash
import os
os.environ["GOOGLE_API_KEY"] = "your_google_key"
os.environ["OPENAI_API_KEY"] = "your_openai_key"
```

## 📌 Usage Example

query = "What is the application of prompting in NLP?"

### Step 1: Retrieve supporting context
### Step 2: Answer with Gemini Pro using LangChain Tool
### Step 3: Evaluate for hallucinations

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

## 📖 Read the Full Article

📝 I’ve documented the full journey, technical architecture, and key learnings in this Medium blog:

👉 [Read on Medium](https://medium.com/@adamya1998official/fakebuster-get-your-facts-right-7000bf3ae881)


## 📜 License
- MIT License – open for learning, research, and adaptation.
