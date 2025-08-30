# AutoGPTnedict 🎬

An AI-powered YouTube content generation tool that creates video titles and scripts using LangChain, OpenAI, and Wikipedia research.

## Overview
AutoGPTnedict is a Streamlit web application that automates the YouTube content creation process. Simply provide a topic, and the app will generate an engaging video title, conduct Wikipedia research, and produce a complete video script based on the research findings.

## Features
- **Automated Title Generation**: Creates catchy YouTube video titles based on your topic
- **Wikipedia Integration**: Automatically researches your topic using Wikipedia API
- **Script Writing**: Generates comprehensive video scripts incorporating research data
- **Conversation Memory**: Maintains history of generated titles and scripts
- **Interactive UI**: Clean Streamlit interface with expandable sections for history and research

## Tech Stack
- **Frontend**: Streamlit
- **LLM Framework**: LangChain
- **AI Model**: OpenAI GPT
- **Research Source**: Wikipedia API
- **Language**: Python 3.8+

## Prerequisites
- Python 3.8 or higher
- OpenAI API key
- Active internet connection (for Wikipedia API)

## Installation

### 1. Clone the Repository
```bash
git clone <repository-url>
cd autogptnedict
```

### 2. Create Virtual Environment
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Set Up API Key
Create a file named `apikey.py` in the project root:
```python
apikey = "your-openai-api-key-here"
```

**Note**: Never commit your API key to version control. Add `apikey.py` to `.gitignore`.

## Requirements File
Create a `requirements.txt` file with:
```txt
streamlit
langchain
openai
wikipedia-api
python-dotenv
```

## Usage

### Running the Application
```bash
streamlit run app.py
```

The app will open in your default browser at `http://localhost:8501`

### How to Use
1. Enter your topic or idea in the text input field
2. Press Enter or click outside the input field
3. Wait for the AI to generate:
   - A YouTube video title
   - Wikipedia research on the topic
   - A complete video script
4. View results in expandable sections:
   - **Title History**: All generated titles in the session
   - **Script History**: All generated scripts
   - **Wikipedia Research**: Raw research data used

## Project Structure
```
autogptnedict/
├── app.py                 # Main Streamlit application
├── apikey.py             # OpenAI API key (not in repo)
├── requirements.txt      # Project dependencies
├── .gitignore           # Git ignore file
└── README.md            # Project documentation
```
