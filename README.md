# Local PDFs Chatbot
The Local PDFs Chatbot is an interactive application built using Streamlit, designed to answer questions based on the content extracted from uploaded PDF documents. It utilizes various machine learning and natural language processing libraries to process the text, generate embeddings, and retrieve relevant information to user queries.


## Features
- **PDF Text Extraction:** Extracts text from uploaded PDF documents.
- **Text Chunking:** Splits the extracted text into manageable chunks for processing.
- **Vector Store Creation:** Generates embeddings for the text chunks and stores them in a FAISS index for efficient similarity search.
- **Conversational Interface:** Engages with the user in a conversational manner, allowing them to ask questions about the content of the PDFs.
- **Responsive UI:** Built with Streamlit, providing an easy-to-use web interface.


## Prerequisites
Before you can run the chatbot, make sure you have the following installed:

- Python 3.8 or later
- Streamlit
- dotenv
- PyPDF2
- langchain (and its dependencies)
- FAISS


## Usage
To start the chatbot, run the following command in your terminal:

**`streamlit run <script-name>.py`**


Once the application is running, follow these steps:

1. **Upload PDFs:** Use the sidebar to upload one or more PDF documents you want to query.
2. **Process PDFs:** Click the 'Process' button to extract text, generate embeddings, and prepare the chatbot for answering questions.
3. **Ask Questions:** Enter your questions in the text input field and receive responses based on the content of the uploaded PDFs.


## Customization
- You can customize the embeddings and the language models used for generating responses by modifying the get_vectorstore and get_conversation_chain functions.
- The appearance and layout of the chat interface can be adjusted by editing the HTML templates and CSS provided in htmlTemplates.py.


## Acknowledgements
This project utilizes several open-source libraries and resources, including Streamlit, langchain, and Hugging Face Transformers. We are grateful to their contributors and maintainers.
