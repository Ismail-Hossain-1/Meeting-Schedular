# Flask Chatbot API with Google Generative AI

This project implements a Flask-based API that integrates with Google's Generative AI (Gemini 1.5) to handle chatbot conversations. The API allows users to interact with the bot and schedule meetings using a custom function. The backend is built using Flask and the Google Generative AI API.

## Features

- **Chatbot Integration**: The app uses Google Generative AI to generate responses based on user input.
- **Meeting Scheduler**: The chatbot is configured with a system instruction to act as an expert in meeting scheduling.
- **User-specific Chat History**: Each user interaction is stored in `chat_history` to maintain context across messages.
- **CORS Support**: The app supports Cross-Origin Resource Sharing (CORS) for flexible interaction across different origins.

## Requirements

To run this application, you need to have the following installed:

- Python 3.x
- `pip` (Python package installer)

### Install Dependencies

1. Clone the repository:

    ```bash
    git clone https://github.com/your-repo/chatbot-api.git
    cd chatbot-api
    ```

2. Install required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

    The `requirements.txt` should contain the following dependencies:

    ```text
    Flask==2.2.2
    flask-cors==3.1.1
    python-dotenv==0.19.2
    google-generativeai==0.1.0
    ```

3. You will also need to set up a `.env` file to store your sensitive credentials, including the Google API key.

## Setup

1. **Create `.env` File**:
   
   In the root directory of the project, create a `.env` file and add the following line:

   ```env
   GOOGLE_API_KEY=your_google_api_key_here
