# WEEK 3 – LLM Monitoring with MongoDB

## 1. Aim
To monitor LLM requests by tracking token usage, response latency, estimated API cost, and storing request details in MongoDB.

## 2. Technologies Used
- Python
- Gemini API
- Ollama
- MongoDB Atlas
- PyMongo
- Requests
- Python-dotenv

## 3. Folder Structure

```text
WEEK3/
├── main.py
├── llm_client.py
├── usage_logger.py
├── test_client.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

## 4. Installation

Activate the shared virtual environment:

```powershell
cd C:\GENAI
.\venv\Scripts\Activate.ps1
```

Navigate to Week 3:

```powershell
cd PRACTICAL\WEEK3
```

Install dependencies:

```powershell
pip install -r requirements.txt
```

## 5. Configuration

Create a `.env` file and configure:

```env
GEMINI_API_KEY=your_api_key
MONGODB_URI=your_mongodb_connection_string
GEMINI_INPUT_PRICE_PER_MILLION=0
GEMINI_OUTPUT_PRICE_PER_MILLION=0
```

Replace the example values with your actual credentials. Never upload `.env` to GitHub.

## 6. MongoDB Configuration

1. Create or open a MongoDB Atlas cluster.
2. Configure a database user.
3. Configure network access.
4. Copy the MongoDB connection string.
5. Add it to `.env`.

Database:

```text
llm_monitoring
```

Collection:

```text
api_usage
```

## 7. Implementation Steps

1. Capture input and output token usage.
2. Measure request latency.
3. Estimate hosted API cost using configurable token rates.
4. Store successful and failed requests in MongoDB.
5. Implement request timeouts and limited retries.

## 8. Execution

Run:

```powershell
python main.py
```

Select a provider:

```text
ollama
```

or

```text
gemini
```

Enter your question.

## 9. Sample Input

```text
Explain Artificial Intelligence with five real-life examples.
```

## 10. Expected Output

The application displays:
- LLM response
- Latency
- Input tokens
- Output tokens
- Total tokens
- Estimated cost

Successful database logging displays:

```text
Usage details saved to MongoDB.
```

## 11. Database Verification

Open MongoDB Atlas and navigate to:

```text
llm_monitoring
    └── api_usage
```

Check the stored documents for provider, model, prompt, response, token usage, latency, estimated cost, status, and timestamp.

## 12. Testing

Run:

```powershell
python -m unittest test_client.py
```

Expected result:

```text
Ran 1 test
OK
```

## 13. Result

Successfully implemented LLM monitoring with token tracking, latency measurement, cost estimation, retry handling, and MongoDB storage.
