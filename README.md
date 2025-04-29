# Image-2-Text: Smart Document Intelligence

A web application that extracts and analyzes text and visual information from images using Azure OpenAI's vision capabilities (GPT-4.1 Vision).

## Overview

Image-2-Text is a document intelligence tool that allows users to upload images containing text, charts, graphs, or other visual information and receive detailed textual descriptions and analysis. The application leverages Azure OpenAI's powerful vision model to understand and interpret image content.

## Features

- **Image Analysis**: Upload images and receive detailed text descriptions of their content
- **Customizable Prompts**: Tailor the analysis by providing specific prompts to focus on particular aspects of the image
- **Support for Various Formats**: Works with common image formats (JPG, JPEG, PNG, BMP)
- **Responsive Web Interface**: Clean, modern UI for desktop and mobile devices
- **Markdown Rendering**: Results are formatted cleanly with markdown support

## Technology Stack

- **Backend**: FastAPI (Python)
- **Frontend**: HTML, CSS, JavaScript
- **AI Service**: Azure OpenAI GPT-4.1 Vision
- **Deployment**: Uvicorn ASGI server

## Requirements

- Python 3.10+
- Azure OpenAI API access with GPT-4.1 Vision capability
- Required Python packages (see requirements.txt)

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/image-2-text.git
   cd image-2-text
   ```

2. Create and activate a virtual environment:
   ```
   python -m venv env
   source env/bin/activate  # On Windows, use: env\Scripts\activate
   ```

3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the project root with your Azure OpenAI configuration:
   ```
   AZURE_OPENAI_API_KEY=your_api_key
   AZURE_OPENAI_ENDPOINT=your_endpoint_url
   AZURE_OPENAI_API_VERSION=2024-12-01-preview
   AZURE_OPENAI_DEPLOYMENT_NAME=your_deployment_name
   ```

## Usage

1. Start the server:
   ```
   python api.py
   ```

2. Open your browser and navigate to:
   ```
   http://localhost:8000
   ```

3. Upload an image or use the default sample
4. Customize the prompt if needed
5. Click "Extract Info" to get the analysis

## Example Use Cases

- Extracting text from documents, charts, and diagrams
- Analyzing graphs and visualizing data in textual format
- Interpreting charts and tables in reports
- Transcribing text from screenshots or photos
- Understanding complex visual information through AI-generated descriptions

## Architecture

The application follows a simple client-server architecture:
- FastAPI backend handles image uploads and communication with Azure OpenAI
- Frontend provides an intuitive interface for uploading images and viewing results
- Azure OpenAI processes the images with its vision capabilities

## Demo

The application comes with a sample stock chart (Microsoft stock price) for immediate testing without uploading your own image.

## License

[Add your license information here]

## Contact

[Add your contact information here]

---

**Note**: This application requires a valid Azure OpenAI API key with access to the GPT-4.1 Vision model.