# AI Video Assistant

An intelligent meeting-analysis system that converts YouTube videos and audio recordings into searchable, multilingual meeting insights.

## Project Overview

**AI Video Assistant** uses Speech-to-Text, Large Language Models, and Retrieval-Augmented Generation (RAG) to analyze meeting recordings. It generates transcripts, summaries, action items, key decisions, and answers user questions based on the recorded content.

## Key Features

* 🎙️ Audio and YouTube video processing
* 📝 Multilingual and Hinglish transcription
* 🤖 AI-powered meeting summarization
* 📌 Action items and key decision extraction
* ❓ Open questions identification
* 🔍 Semantic search using RAG
* 💬 Context-aware question answering
* 📚 ChromaDB-based vector storage
* 🌐 Interactive Streamlit interface

## Tech Stack

* **Programming:** Python
* **Speech-to-Text:** Whisper, Sarvam AI
* **LLM:** Mistral AI
* **Framework:** LangChain
* **Embeddings:** HuggingFace, Sentence Transformers
* **Vector Database:** ChromaDB
* **Frontend:** Streamlit
* **Architecture:** Retrieval-Augmented Generation (RAG)

## Workflow

```text
YouTube Video / Audio
        ↓
Audio Extraction
        ↓
Speech-to-Text
(Whisper / Sarvam AI)
        ↓
Transcript Generation
        ↓
Text Chunking & Embeddings
        ↓
ChromaDB Vector Database
        ↓
Mistral AI + LangChain
        ↓
Summary / Insights / Q&A
        ↓
Streamlit Dashboard
```

## Project Structure

```text
AI-Video-Assistant/
│
├── app.py
├── requirements.txt
├── README.md
├── .env
│
├── src/
│   ├── components/
│   ├── prompts/
│   ├── utils/
│   └── ...
│
├── data/
└── chroma_db/
```

## Installation

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
cd AI-Video-Assistant
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file and add the required API keys:

```env
MISTRAL_API_KEY=your_mistral_api_key
SARVAM_API_KEY=your_sarvam_api_key
```

### 5. Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

## Use Cases

* Meeting summarization
* Lecture and educational video analysis
* Multilingual meeting transcription
* Action-item extraction
* Knowledge retrieval from long recordings
* Conversational analysis of meeting content

## Future Enhancements

* Speaker identification
* Automatic meeting minutes generation
* Export reports as PDF
* User authentication
* Advanced analytics dashboard
* Support for additional video platforms
* Improved multilingual capabilities

## License

This project is developed for educational and demonstration purposes.
