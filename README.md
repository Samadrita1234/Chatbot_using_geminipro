# Chatbot_using_geminipro
This Streamlit-based application allows users to interact with PDF documents by asking questions and receiving context-aware answers powered by Google's Gemini AI. Users can upload multiple PDF files, from which the text is extracted using PyPDF2 and split into manageable chunks with LangChain's RecursiveCharacterTextSplitter. The text chunks are embedded using Google's Generative AI Embeddings and stored in a FAISS vector database for efficient similarity searches. When a user inputs a question, the system retrieves the most relevant text chunks through similarity search and uses a custom prompt with Gemini AI to generate an accurate response based on the provided context. The app combines document processing, vector search, and conversational AI to enable seamless Q&A interaction with PDF content.

Workflow:
Upload PDFs ➔ Extract Text ➔ Split Text into Chunks ➔ Generate Embeddings ➔ Store in FAISS.
User Asks a Question ➔ Retrieve Relevant Context via Similarity Search ➔ Generate Answer with Gemini AI.
This allows users to interact with PDF content conversationally, extracting answers based on their queries using context-aware AI.
