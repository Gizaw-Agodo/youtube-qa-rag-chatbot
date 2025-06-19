# YouTube Transcript Question-Answering

This project demonstrates how to fetch a YouTube video transcript, chunk and embed it, then use a LangChain-based pipeline with OpenAI’s GPT-4o-mini model to answer questions based only on the transcript.

## Features

- Fetch video transcript using `youtube-transcript-api`
- Split transcript into chunks for better context handling
- Embed chunks and store in FAISS vector store
- Retrieve relevant transcript parts by similarity search
- Use a prompt template to guide GPT-4o-mini to answer questions
- End-to-end chain combining retrieval and generation

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/youtube-qa-rag-chatbot.git
   cd youtube-qa-rag-chatbot
   ```
2. Create and activate a Python environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```
3. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```
4. Add your OpenAI API key to a `env` file:
   ```ini
   OPENAI_API_KEY=your_openai_api_key_here
   ```
5. Open the notebook `transcript_qa.ipynb` in Jupyter and run the cells.

## Dependencies

- Python 3.8+
- langchain
- youtube-transcript-api
- faiss-cpu
- python-dotenv
- openai (via LangChain)

