
# Chat with Websites

## Overview

This project is a Streamlit web application that allows users to chat with the content of a given website. It leverages the Langchain framework to split the website content into chunks, create a vector store, and perform conversational retrieval-augmented generation (RAG). Additionally, it includes sentiment analysis on the website's content.

## Features

- **Chat with Website Content**: Extract and interact with the content of a specified website.
- **Conversational RAG**: Perform history-aware retrieval and generate responses based on the retrieved context.
- **Sentiment Analysis**: Analyze the sentiment polarity and subjectivity of the website's content.

## Repository Structure

\`\`\`plaintext
.
├── .chroma
├── src
│   └── app.py
├── .env
├── .gitignore
└── requirements.txt
\`\`\`

## Installation

1. **Clone the repository**
   \`\`\`bash
   git clone <repository-url>
   cd <repository-directory>
   \`\`\`

2. **Set up the environment**
   - Using `pip`:
     \`\`\`bash
     pip install -r requirements.txt
     \`\`\`

3. **Run the application**
   \`\`\`bash
   streamlit run src/app.py
   \`\`\`

## Usage

### Configuration

- **Website URL**: Enter the URL of the website you want to interact with in the sidebar.

### Chat with the Website

1. Enter a valid website URL in the sidebar.
2. Type your message in the chat input box.
3. The bot will respond based on the content of the website.

### Sentiment Analysis

- The application will display the sentiment polarity and subjectivity of the website's content in the main area.

## Example

1. **Enter Website URL**: `https://example.com`
2. **Chat**:
   - User: "What is the main topic of this website?"
   - AI: "The main topic of this website is..."

3. **Sentiment Analysis**:
   - Sentiment Polarity: `0.1`
   - Sentiment Subjectivity: `0.4`

## Things to Fix or Add

### Fixes

1. **Error Handling**:
   - Improve error handling for network issues and invalid URLs.

2. **Documentation for Functions**:
   - Add docstrings for all functions to improve readability and maintainability.

3. **API Key Management**:
   - Securely manage API keys, possibly using environment variables or a configuration file.

### Additions

1. **Unit Tests**:
   - Add unit tests for the data extraction and processing functions to ensure reliability.

2. **Improved UI**:
   - Enhance the Streamlit interface with better layout and styling for a more user-friendly experience.

3. **Caching**:
   - Implement caching for API responses to improve performance and reduce the number of API calls.

4. **Expanded Data Sources**:
   - Include additional data sources or APIs to provide a broader range of content.

5. **Interactive Charts**:
   - Add more interactive elements to charts, such as tooltips and filters.

## Contribution

Feel free to contribute by opening issues, submitting pull requests, or providing feedback.

## License

This project is licensed under the MIT License.
