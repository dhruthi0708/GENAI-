# WEEK 1 – Gemini API Integration

## Aim
To connect a Python application with Google's Gemini API and generate AI responses using prompts.

## Technologies Used
- Python
- Google Gemini API
- Google GenAI SDK
- VS Code
- Environment Variables (`.env`)

## Tools Used
- Python
- Visual Studio Code
- Gemini API

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

1. Install Python on your system.
2. Open the WEEK1 folder in VS Code.
3. Install the required packages:

```bash
pip install -r requirements.txt
```

4. Create a `.env` file and add your Gemini API key:

```text
GEMINI_API_KEY=your_api_key_here
```

**Note:** Never upload your actual API key to GitHub.

## Execution Steps

Run the following command in the terminal:

```bash
python main.py
```

1. The program connects to the Gemini API.
2. Enter a prompt or question.
3. The prompt is sent to the Gemini model.
4. The model generates a response.
5. The response is displayed in the terminal.

## Expected Output

The program displays an AI-generated response based on the prompt entered by the user.

**Example:**

Input:
```text
What is Artificial Intelligence?
```

Output:
```text
Artificial Intelligence is a branch of computer science
that enables machines to perform tasks that normally
require human intelligence.
```

## Result
Successfully connected a Python application with Google's Gemini API and generated AI responses using user-provided prompts.
