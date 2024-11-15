# DebugMate - AI Code Reviewer

DebugMate is a simple web app built using Streamlit and Google's Gemini API to review code and identify potential bugs. It allows users to input their code, get an AI-generated review, and receive suggestions for improvements or bug fixes.

## Features:
- AI-driven code review using Google Gemini API.
- Detects and reports potential bugs or issues in the provided code.
- Supports multiple programming languages, providing a review based on the language of the code.

---

## Requirements

Before running the app, ensure you have the following installed:

- Python 3.x
- Streamlit
- `python-dotenv`
- Google Gemini API client (`google-generativeai`)

You can install the necessary Python packages by running the following command:

```bash
pip install streamlit python-dotenv google-generativeai
```

---

## Setup

1. **Clone the repository** (or download the files).

2. **Create a `.env` file** in the root directory and add the following line with your Google Gemini API key:

   ```
   GOOGLE_API_KEY=your_google_api_key
   ```

   You can obtain the API key from the [Google Gemini API documentation](https://developers.google.com/gemini) (or wherever you got your API key).

3. **Run the app** using Streamlit:

   ```bash
   streamlit run app.py
   ```

   This will start the app in your browser.

---

## How to Use

1. Once the app is running, you’ll see a text area where you can input your code.
2. After entering the code, click the "Review my code →" button.
3. The app will analyze the code and provide a bug report, including any issues found.
4. If the API key is missing or the code is not entered, the app will prompt you accordingly.

---

## Troubleshooting

- **API Key Missing:** Ensure that your `.env` file contains the correct `GOOGLE_API_KEY`.
- **Error Messages:** If an error occurs during code review, check the error message displayed on the app, which can help you troubleshoot the issue.
