
# BioMistral Medical RAG Chatbot


## Overview

The **BioMistral Medical RAG Chatbot** is a Retrieval-Augmented Generation (RAG) based chatbot designed specifically for the medical domain. This project leverages the power of **BioMistral**, an open-source large language model (LLM) optimized for handling biomedical data. By combining document retrieval with advanced language modeling, the chatbot provides accurate, context-aware responses to medical queries by drawing from trusted medical literature.

## Key Features

- **Biomedical Focus**: Utilizes domain-specific biomedical documents to answer queries with high relevance and accuracy.
- **Document-Based Retrieval**: Capable of retrieving relevant information from biomedical texts, such as research papers, clinical guidelines, and more.
- **BioMistral LLM**: Employs the BioMistral-7B LLM, a state-of-the-art language model trained for medical applications.
- **Efficient Query Handling**: The chatbot can process complex medical questions and provide factual responses, improving over time as it incorporates more documents.
- **Interactive Mode**: Supports real-time query handling for interactive chatbot experiences.

## Use Cases

- **Medical Assistance**: Provides support for healthcare professionals and patients by answering common medical questions.
- **Research Aid**: Assists researchers by quickly retrieving information from large collections of biomedical papers.
- **Medical Education**: A learning tool for students in the medical field to enhance their understanding of medical concepts through a question-and-answer format.

## How It Works

The chatbot uses **RAG (Retrieval-Augmented Generation)**, which is a hybrid approach combining the retrieval of relevant documents with the generation of natural language answers. The key steps involved are:

1. **Document Loading**: Uploads biomedical documents in PDF format, which the chatbot uses as a source of knowledge.
2. **Document Chunking**: Splits large documents into smaller, manageable chunks for efficient search and retrieval.
3. **Semantic Embeddings**: Transforms the document chunks into dense vectors using a pre-trained **PubMedBERT** model. This allows the system to understand the semantic meaning of queries and documents.
4. **Vector Store**: Stores the vector representations of document chunks in a vector database, enabling fast and accurate similarity-based search.
5. **Query Processing**: When a user submits a query, the system retrieves the most relevant chunks of text based on semantic similarity.
6. **Response Generation**: The chatbot uses the retrieved information to generate a well-informed and contextually accurate response using the BioMistral LLM.

## Setup and Installation

To set up the project, you will need to:

1. Install the required Python libraries.
2. Mount your cloud storage (e.g., Google Drive) for data access.
3. Load biomedical PDFs into the appropriate folder.
4. Configure your **BioMistral-7B** model and connect it to the RAG chain.
5. Interact with the chatbot via command-line or in a notebook environment for real-time queries.

More detailed setup instructions can be found in the `SETUP.md` file in the repository.



## Technologies Used

- **LangChain**: For handling document loaders, text splitting, and chains.
- **Sentence-Transformers**: To create high-quality embeddings from biomedical text.
- **ChromaDB**: A vector store for managing and querying document chunks.
- **BioMistral LLM**: The backbone language model for generating accurate medical responses.
- **LlamaCpp**: A framework to efficiently run the BioMistral model.
- **Hugging Face**: API for model integration and embedding creation.

## Limitations and Future Work

While the BioMistral Medical RAG Chatbot provides a robust framework for answering medical questions, there are a few limitations to consider:

- **Scope**: The chatbot relies heavily on the quality and scope of the documents loaded into its system. Expanding the document base could improve the quality of responses.
- **Model Size**: The BioMistral-7B model is large and may require significant computational resources. Exploring model optimization techniques could reduce resource consumption.
- **Real-Time Adaptation**: Future versions may include fine-tuning capabilities to allow the chatbot to learn and adapt based on user feedback and new data.

## Contributing

We welcome contributions from the community! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch with your feature or bugfix.
3. Submit a pull request detailing your changes.

For major changes, please open an issue first to discuss what you would like to change.



