# RAG System

A modular Retrieval-Augmented Generation (RAG) system that combines document retrieval with large language models to provide accurate and contextual responses.

## Project Structure

```
rag-system/
├── src/                    # Main source code directory
│   ├── __init__.py
│   ├── api/               # API endpoints and interfaces
│   ├── embedding/         # Text embedding functionality
│   ├── generation/        # Text generation components
│   ├── preprocessing/     # Document preprocessing pipeline
│   ├── retrieval/         # Document retrieval components
│   ├── utils/            # Utility functions and helpers
│   └── vector_store/     # Vector database management
├── data/                  # Data storage directory
│   ├── documents/        # Raw documents storage
│   └── embeddings/       # Processed embeddings storage
├── config/               # Configuration files
│   ├── config.yaml       # Main configuration
│   └── .env.template     # Environment variables template
├── tests/                # Test files
├── docs/                 # Documentation
├── scripts/              # Setup and utility scripts
└── requirements.txt      # Python dependencies
```

## Features

- **Document Preprocessing**: Clean and chunk documents for optimal retrieval
- **Text Embeddings**: Generate semantic embeddings using transformer models
- **Vector Storage**: Efficient storage and retrieval using vector databases
- **Document Retrieval**: Smart document retrieval based on semantic similarity
- **Text Generation**: Context-aware response generation using LLMs
- **API Interface**: RESTful API for easy integration

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/Software-TutorAI-Comu/rag-system.git
   cd rag-system
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure environment**
   ```bash
   cp config/.env.template .env
   # Edit .env with your API keys and configuration
   ```

4. **Run the system**
   ```bash
   # Add your documents to data/documents/
   # Start the API server
   python -m src.api.main
   ```

## Configuration

The system can be configured through:
- `config/config.yaml`: Main configuration file
- `.env`: Environment variables (API keys, secrets)

## Modules

### Retrieval (`src/retrieval/`)
Handles document indexing, similarity search, and query processing.

### Generation (`src/generation/`)
Manages language model integration and response generation.

### Embedding (`src/embedding/`)
Provides text embedding generation and similarity computation.

### Vector Store (`src/vector_store/`)
Manages vector database operations and similarity search.

### Preprocessing (`src/preprocessing/`)
Handles document cleaning, chunking, and format conversion.

### API (`src/api/`)
Provides REST API endpoints for system interaction.

### Utils (`src/utils/`)
Contains utility functions, configuration management, and logging.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests
5. Submit a pull request

## License

This project is open source and available under the MIT License.