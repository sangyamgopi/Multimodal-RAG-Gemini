# Multimodal RAG using Gemini

A Multimodal Retrieval-Augmented Generation (RAG) system that allows users to ask questions about PDF documents containing both text and images.

The system uses CLIP for text and image embeddings, FAISS for similarity-based retrieval, and Google's Gemini model to generate context-aware answers.

## 🚀 Project Overview

Traditional RAG systems mainly focus on retrieving information from text. This project extends the approach by processing both textual and visual content from PDF documents.

Users can ask natural-language questions and receive answers based on relevant text and images retrieved from the document.

## ✨ Features

- Extracts text and images from PDF documents.
- Generates text and image embeddings using CLIP.
- Stores and retrieves relevant content using FAISS.
- Uses Gemini to generate context-aware answers.
- Supports questions about charts, images, and textual information.
- Provides document-based question answering.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| PyMuPDF | PDF text and image extraction |
| Hugging Face CLIP | Text and image embeddings |
| FAISS | Vector similarity search |
| Google Gemini | Answer generation |
| LangChain | LLM integration |
| PyTorch | Deep learning framework |
| Jupyter Notebook | Development environment |

## 🏗️ System Architecture

1. **PDF Input:** Load a PDF containing text and images.
2. **Content Extraction:** Extract text and images using PyMuPDF.
3. **Embedding Generation:** Generate 512-dimensional text and image embeddings using CLIP.
4. **Vector Storage:** Store embeddings in a FAISS vector database.
5. **Retrieval:** Retrieve relevant text and images based on the user's query.
6. **Answer Generation:** Pass the retrieved context to Gemini to generate the final answer.

## 🔄 Workflow

PDF Document → PyMuPDF → CLIP Embeddings → FAISS Retrieval → Gemini → Final Answer

## 📂 Project Structure

```text
Multimodal-RAG-Gemini/
│
├── main.ipynb
├── requirements.txt
├── sample.pdf
├── .gitignore
├── .env (not uploaded)
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/sangyamgopi/Multimodal-RAG-Gemini.git
```

### 2. Navigate to the project directory

```bash
cd Multimodal-RAG-Gemini
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Configure Gemini API key

Create a `.env` file in the project directory:

```env
GOOGLE_API_KEY=your_gemini_api_key
```

Get your API key from [Google AI Studio](https://aistudio.google.com/apikey).

**Never share or upload your API key to GitHub.**

### 6. Run the notebook

Open `main.ipynb` in Jupyter Notebook or VS Code and execute the cells.

## 💡 Example Questions

- What does the chart on page 1 show about revenue trends?
- Summarize the main findings from the document.
- Describe the chart or image in the PDF.
- What is the main topic of the document?

## 🎯 Applications

- Financial report analysis
- Educational document understanding
- Business report analysis
- Research paper exploration
- Question answering from image-rich PDF documents

## 🔮 Future Improvements

- Build an interactive web application using Streamlit.
- Support multiple PDF uploads.
- Improve retrieval accuracy.
- Add chat history and conversational question answering.
- Support larger and more complex documents.

## 👨‍💻 Author

**Sangyam Gopi**

GitHub: [@sangyamgopi](https://github.com/sangyamgopi)

---

If you find this project useful, feel free to ⭐ the repository!
