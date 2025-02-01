# LM Studio Response Streamer

LM Studio Response Streamer is a user-friendly desktop application that lets you interact with AI language models through LM Studio's API.

With its clean and intuitive interface, you can customize system prompts, adjust parameters like temperature and token limits, and see AI responses stream in real-time with markdown-style formatting.

The app features a simple setup process, model selection capabilities, and the ability to stop generation at any time, making it perfect for anyone looking to experiment with local AI models without dealing with complex technical configurations.

## Features

- Real-time response streaming from LM Studio
- Customizable system messages and user prompts
- Adjustable parameters (temperature, max tokens)
- Model selection dropdown
- Clean and intuitive GUI built with tkinter
- Markdown-like text formatting in responses
- Stop generation functionality

## Prerequisites

- Python 3.x
- LM Studio running locally or on a remote server
- Required Python packages (see requirements below)

## Installation

1. Clone this repository
2. Install the required packages:
```bash
pip install requests python-dotenv tkinter
```

3. Copy `.env-example` to `.env` and configure your settings:
```bash
API_IP=127.0.0.1  # IP address of your LM Studio server
PORT=1234         # Port of your LM Studio server
```

## Usage

1. Start LM Studio and ensure it's running with the API server enabled
2. Run the application:
```bash
python main.py
```

3. Configure your settings in the GUI:
   - Enter a system message (default: "You are a helpful AI assistant.")
   - Type your user message
   - Adjust temperature and max tokens as needed
   - Select your preferred model from the dropdown
   - Click "Generate" to start generation
   - Use "Stop" to halt generation at any time

## Configuration

The application uses environment variables for configuration:
- `API_IP`: The IP address of your LM Studio server
- `PORT`: The port number of your LM Studio server

## Features in Detail

- **System Message**: Sets the context for the AI model
- **User Message**: Your input prompt for the AI
- **Temperature**: Controls response randomness (0.0 - 1.0)
- **Max Tokens**: Limits response length (-1 for no limit)
- **Model Selection**: Choose from available LM Studio models
- **Real-time Streaming**: See responses as they're generated
- **Stop Generation**: Cancel generation at any time

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License. 