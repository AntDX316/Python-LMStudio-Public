# Python LM Studio GUI

Python LM Studio GUI is a powerful desktop application that brings a user-friendly interface to LM Studio's AI capabilities.

This elegant tool allows you to interact with large language models through a simple graphical interface, featuring real-time streaming responses, customizable system prompts, and adjustable parameters like temperature and token limits.

With built-in support for function calling and markdown-formatted responses, it makes AI interaction accessible while maintaining advanced features that power users expect.

Whether you're testing prompts, generating content, or exploring AI capabilities, this application provides a seamless bridge between you and LM Studio's powerful language models.

## Features

- 🤖 Compatible with LM Studio's API
- 💬 Support for system and user messages
- 🔄 Real-time streaming responses
- 🛠️ Function calling support
- 🎛️ Adjustable parameters (temperature, max tokens)
- 🎨 Markdown-style formatting in responses
- ⏹️ Stop generation at any time

## Setup

1. Install and start LM Studio:
   - Download LM Studio from [https://lmstudio.ai/](https://lmstudio.ai/)
   - Start the local server in LM Studio
   - Load your desired model

2. Clone and install dependencies:
```bash
git clone https://github.com/yourusername/Python-LMStudio.git
cd Python-LMStudio
pip install -r requirements.txt
```

3. Configure environment:
```bash
cp .env-example .env
```
Edit `.env` file and set:
- `API_IP`: IP address of your LM Studio server (default: 127.0.0.1)
- `PORT`: Port number (default: 1234)

4. Start the application:
```bash
python main.py
```

## Usage

1. **System Message**: Set a system message to define the AI's behavior or context (optional)

2. **User Message**: Enter your prompt or question

3. **Parameters**:
   - Temperature: Controls response randomness (0.0 to 1.0)
   - Max Tokens: Limits response length (-1 for no limit)

4. **Model Selection**: Choose from available LM Studio models

5. **Controls**:
   - Generate: Start generating a response
   - Stop: Stop the current generation

## Function Calling

The application includes a sample product search function that demonstrates LM Studio's function calling capabilities:

```python
{
    "name": "search_products",
    "description": "Search the product catalog by various criteria",
    "parameters": {
        "query": "Search terms or product name",
        "category": ["electronics", "clothing", "home", "outdoor"],
        "max_price": "Maximum price in dollars"
    }
}
```

## Requirements

- Python 3.x
- LM Studio
- Required Python packages:
  - requests==2.31.0
  - python-dotenv==1.0.1

## License

This project is licensed under the MIT License.
