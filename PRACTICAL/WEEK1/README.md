# WEEK 1 – Gemini API Integration

## Aim
To connect a Python application with Google's Gemini API and generate AI responses using prompts.

## Technologies Used
- Python
- Google Gemini API
- Google GenAI SDK
- VS Code

## Folder Structure
```text
WEEK1/
├── main.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

## Installation Steps
1. Install Python.
2. Open the project in VS Code.
3. Activate the Python virtual environment.
4. Install the required packages:

```bash
pip install -r requirements.txt
```

## API Configuration
Create a `.env` file and configure your Gemini API key:

```env
GEMINI_API_KEY=your_api_key
```

Never upload your actual API key to GitHub.

## Execution
Run the program:

```bash
python main.py
```

Enter a question when prompted.

## Sample Input
```text
Explain Artificial Intelligence in simple words.
```

## Expected Output
The program displays an AI-generated explanation of Artificial Intelligence.

## Result
Successfully connected Python with the Gemini API and generated AI responses using user prompts.
