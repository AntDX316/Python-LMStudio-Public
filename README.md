https://lmstudio.ai/

# LM Studio Response Streamer

LM Studio Response Streamer is a sleek, user-friendly desktop application that lets you interact with AI language models running on LM Studio's local server.

With its clean interface, you can easily generate AI responses in real-time, customize model parameters like temperature and token length, and use system prompts to guide the AI's behavior.

Perfect for developers, writers, and AI enthusiasts who want to work with local AI models without dealing with command-line interfaces or complex setups.

The app features real-time streaming of responses, a model selection dropdown, and the ability to stop generation at any time, making it an ideal tool for both quick queries and longer AI-assisted writing sessions.

## Features

- Modern Tkinter-based GUI interface
- Real-time response streaming
- Configurable model parameters (temperature, max tokens)
- Support for system messages and user prompts
- Model selection dropdown
- Stop generation functionality
- Clean, system-native look and feel

## Prerequisites

- Python 3.x
- LM Studio running locally or on a remote server
- Required Python packages (see requirements below)

## Installation

1. Clone this repository:
```bash
git clone [repository-url]
cd [repository-name]
```

2. Install the required packages:
```bash
pip install requests python-dotenv tkinter
```

3. Copy the `.env-example` file to `.env` and configure your settings:
```bash
cp .env-example .env
```

4. Edit the `.env` file with your LM Studio server details:
```
API_IP=127.0.0.1  # or your LM Studio server IP
PORT=1234         # or your LM Studio server port
```

## Usage

1. Start LM Studio and ensure the API server is running
2. Run the application:
```bash
python main.py
```

3. In the application:
   - Enter your system message (optional)
   - Type your user message
   - Adjust temperature and max tokens as needed
   - Select your desired model
   - Click "Generate" to start generation
   - Use "Stop" to halt generation at any time

## Configuration

- **Temperature**: Controls randomness in the response (0.0 to 1.0)
- **Max Tokens**: Maximum length of the generated response
- **System Message**: Sets the behavior context for the AI
- **Model Selection**: Choose from available LM Studio models

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

[Your License Here]

## Acknowledgments

- Built for use with LM Studio
- Uses the Tkinter library for the GUI
- Implements streaming responses for real-time interaction 