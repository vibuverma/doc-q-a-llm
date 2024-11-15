# Document QA with Google Gemini and Groq

This project demonstrates how to use the Google Gemini and Groq APIs to build a document question answering system.

## Usage

1. Install the required packages with `pip install -r requirements.txt`
2. Create a `.env` file with the following variables:
    * `GOOGLE_API_KEY` - your Google API key
    * `GROQ_API_KEY` - your Groq API key
3. Run the app with `streamlit run app.py`
4. Enter a text prompt and ask a question

## How it works

1. The app loads the PDF file or text prompt and splits it into chunks
2. The chunks are then embedded using the Google Gemini API
3. The embedded chunks are then indexed using the Groq API
4. When a question is asked, the app uses the Groq API to search for relevant chunks
5. The app then uses the Google Gemini API to generate an answer based on the relevant chunks

## Note

This project is for demonstration purposes only and should not be used in production without proper error handling and security measures.
