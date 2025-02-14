# Conversational AI Chatbot

This project implements a chatbot using GPT-4 Turbo, capable of handling both text and image inputs. It includes both a command-line interface (CLI) and a web-based interface using Flask. Users can interact with the chatbot via a simple web UI or directly through the terminal.

## Key Features:

1. **Text and Image Processing**: 
   - Users can send text or image inputs.
   - Images are encoded in Base64 format and processed by the OpenAI API.
   
2. **Command-Line Interface (CLI)**: 
   - Users can chat with the AI assistant directly in the terminal.
   - Supports text input and image uploads via file paths.

3. **Web-Based Chat Interface**: 
   - Built with HTML, JavaScript, and Flask.
   - Uses JavaScript to send user messages or images to the backend API.
   
4. **Flask API**: 
   - Handles user requests and forwards them to OpenAI's GPT-4.
   - Implements content moderation to prevent harmful responses.

## Files Included:
```
/ConversationalAI
│
├── conversational_ai.py  # Backend Flask application
├── index.html      # Chatbot UI
├── README.md       # Project documentation
```

## Requirements:
To run this project, you will need the following Python packages:

- **Flask**: For creating the web server.
- **Flask-CORS**: To enable cross-origin requests.
- **OpenAI**: To interact with the GPT-4 API.
- **Base64**: For encoding and decoding image data.
- **Requests**: To handle HTTP requests.
- **Argparse**: For command-line argument parsing.
- **Python-dotenv**: To securely manage API keys.

You can install them using:
```
pip install flask flask-cors openai requests argparse python-dotenv
```

## How to Run:

### 1. Extract the files from the email/sent attachment and have tehm in same directory.

### 2. Install dependencies: 
```
pip install flask flask-cors openai requests argparse python-dotenv
```

### 3. Run the chatbot:
#### CLI Mode:
```
python conversational_ai.py --mode cli
```
#### Web Mode:
```
python conversational_ai.py --mode web
```
This will start the Flask server at `http://127.0.0.1:5000/chat`.

## Usage:
Once the app is launched, you can:

* Chat with the AI via the command-line interface.
* Interact with the chatbot using the web UI.
* Upload images for AI analysis (in the web UI or CLI mode).

## Example Interaction:

![alt text](/demonstration/demonstration.mp4)



## Notes:
- Need to ensure that your OpenAI API key is valid and kept secure.
- Need to update chatbot's response moderation filters out harmful content.
- You can further expand this project by adding authentication, a database, or voice input.

This chatbot provides a flexible and interactive way to engage with AI, whether via a terminal or web browser.


