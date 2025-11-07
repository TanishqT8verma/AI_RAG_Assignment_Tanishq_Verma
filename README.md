## Local RAG Assistant(by Tanishq Verma)
This project is a document-based question-answering system that lets users upload their own files (PDF, DOCX, TXT, or CSV) and ask questions directly from the content.
It follows a Retrieval-Augmented Generation (RAG) approach — meaning it finds relevant information from your documents and then generates precise answers using an AI model.

## How It Works

- Uploaded documents are read and split into smaller chunks.
- Each chunk is converted into embeddings using SentenceTransformer.
-The vectors are stored in a FAISS database for quick search.
 -When a question is asked, the most relevant chunks are retrieved.
 -A DistilBERT model extracts the best possible answer.
 -Results are shown in a clean Streamlit interface with confidence scores.
Key Libraries

## streamlit – Web interface
sentence-transformers – Text embeddings,
faiss-cpu – Vector search,
transformers – QA model (DistilBERT),
PyPDF2, python-docx, pandas – File handling.
## Example
Input: “What is my name?”
Output:
• tanishq verma  
📊 Confidence: 0.92
