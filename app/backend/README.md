# Backend Service

This directory contains the backend service for the Azure OpenAI and Cognitive Search Demo application. The backend is built using FastAPI and provides APIs for chat interactions, document search, and document analysis using Azure OpenAI and Azure Cognitive Search.

## Project Structure

The backend service is organized into several key components:

- `approaches/` - Contains different implementation approaches for chat and search functionality
- `contracts/` - Data models and contracts for the API
- `services/` - Core services for interacting with Azure OpenAI and Cognitive Search
- `utilities/` - Helper utilities and common functions

## Setup and Configuration

The backend service requires several Azure services to be configured:

- Azure OpenAI
- Azure Cognitive Search
- Azure Storage Account (for document storage)
- Azure App Configuration (optional)

Configuration is handled through environment variables which can be set up using the scripts in the root `/scripts` directory.

## Development

To run the backend service locally:

1. Ensure Python 3.9+ is installed
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Set up required environment variables
4. Run the service:
   - Windows: Use `start.ps1` in the app directory
   - Linux/Mac: Use `start.sh` in the app directory

## API Documentation

When running locally, API documentation is available at:
- Swagger UI: `http://localhost:8000/docs`
- ReDoc: `http://localhost:8000/redoc`

## Testing

Tests for the backend service are located in the `/tests` directory at the root of the project. Run tests using pytest:

```bash
pytest tests/
```
