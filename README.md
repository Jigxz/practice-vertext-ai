# LangSmith App

A Python application demonstrating the use of LangChain with Google Vertex AI's Gemini model for conversational AI.

## Features

- Integration with Google Vertex AI (Gemini 2.5 Flash model)
- Conversational memory management
- Environment variable configuration
- Chat history tracking

## Prerequisites

- Python 3.x
- Google Cloud Project with Vertex AI API enabled
- LangChain API key
- Google Vertex AI credentials
- Additional API keys (Tavily, Groq, Serper)

## Setup

1. Clone the repository
2. Create a `.env` file in the root directory with the following variables:
   ```
   LANGCHAIN_API_KEY=your_langchain_api_key
   VERTEXAI_KEY=your_vertexai_key
   TAVILY_API_KEY=your_tavily_api_key
   GROQ_API_KEY=your_groq_api_key
   VERTEXAI_PROJECT=your_vertexai_project_id
   SERPER_API_KEY=your_serper_api_key
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

The project includes a Jupyter notebook (`practice.ipynb`) that demonstrates:

1. Setting up environment variables
2. Initializing the Vertex AI chat model
3. Making basic queries to the model
4. Implementing conversational memory with chat history

## Example

```python
from langchain_google_vertexai import ChatVertexAI
chat = ChatVertexAI(model="gemini-2.5-flash", project=your_project_id)
response = chat.invoke("Your question here")
```

## Contributing

Feel free to open issues and pull requests to improve the project.

## License

This project is open source and available under the MIT License.