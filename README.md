 
# Local PDF Retrieval-Augmented Generation (RAG) with Llama 3.1
 
This project implements a local PDF Retrieval-Augmented Generation (RAG) solution using the Llama 3.1 model on a Jupyter Notebook. The setup enables extracting content from PDFs and querying it using LLM-powered conversational responses, ensuring privacy by running entirely locally without reliance on external APIs or internet connections.

## Features

- **PDF Content Extraction**: Efficiently parses PDF files to extract textual content.
- **Local LLM Support**: Utilizes Llama 3.1 as a local language model, ensuring data privacy and control.
- **ChromaDB Integration**: Provides a vector store for efficient document indexing and similarity search.
- **LangChain Framework**: Facilitates the RAG pipeline with modules for text splitting, embeddings, and retrieval.

## Prerequisites
 
- **Python** 3.8 or higher
- Jupyter Notebook environment for running `local_RAG.ipynb`

## Installation

1. **install the Ollama framework**  
   
   https://ollama.com/download
 
2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ``` 

### Key Dependencies

- `ollama`: For local model serving.
- `chromadb`: Vector database for document storage and retrieval.
- `pdfplumber`: Parses and extracts text from PDFs.
- `langchain` modules: Manages the RAG pipeline with tools for text processing and querying.
- `unstructured[all-docs]`: Processes diverse document formats.
- `onnx==1.16.1`: Ensures compatibility with specific model requirements.

## Usage

1. **Load the Notebook**: Open `local_RAG.ipynb` in Jupyter Notebook.
2. **Add PDF Files**: Place the PDF files you want to query in the directory specified in the notebook.
3. **Run the Cells**: Execute the cells in sequence to:
   - Parse and process PDF content.
   - Index the extracted text into a vector database.
   - Query the indexed content using Llama 3.1.
4. **Ask Questions**: Use the final cell to input queries based on the PDF content, with responses generated by the LLM model.

## Model Information

This project uses the Llama 3.1 model with the `ollama` framework for local inference. Ensure sufficient computational resources, as running large language models locally may require significant memory and processing power.

## Troubleshooting

- **Memory Requirements**: Running large models locally may require considerable memory. Close other applications if you encounter resource limitations. 