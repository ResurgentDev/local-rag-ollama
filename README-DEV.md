# Local-RAG-Ollama (Enhanced Version)

A production-ready implementation of RAG (Retrieval-Augmented Generation) using Ollama, building on concepts from [local-rag-ollama-basic-demo](https://github.com/ResurgentDev/local-rag-ollama-basic-demo).

## Core Improvements

- Enhanced error handling and recovery
- Improved document matching and relevance scoring
- Flexible configuration options
- Command-line interface
- Progress tracking and logging

## Architecture

### Components
1. Document Fetcher (`fetch_docs.py`)
   - Generic URL handling
   - Multiple document source support
   - Error handling with retries

2. Document Processor (`chunk_docs.py`)
   - Smart chunking strategies
   - Metadata preservation
   - Progress tracking

3. Embedding System (`create_embeddings.py`)
   - Multiple model support
   - Batch processing
   - Caching system

4. Retriever (`setup_retriever.py`)
   - Enhanced index configuration
   - Optimized chunk mapping
   - Index verification

5. Query Engine (`query_model.py`)
   - Advanced relevance scoring
   - Context optimization
   - Enhanced prompt engineering

## Development Status

Current focus:
1. [ ] Error handling improvements
2. [ ] Logging system
3. [ ] Configuration system
4. [ ] Testing framework

## Testing

```bash
# Run tests
python -m pytest tests/

# Run specific test
python -m pytest tests/test_fetch_docs.py
```

## Configuration

Override defaults in `config.py` or use environment variables:
```bash
export RAG_BASE_DIR="/custom/path"
export RAG_MODEL="custom-model"
```
