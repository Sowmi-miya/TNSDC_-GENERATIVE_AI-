# YouTube Video Summarizer

A Python Streamlit web app that summarizes YouTube video content by extracting the transcript and generating a concise summary using a local Hugging Face transformer model.

Features
Extracts transcripts directly from YouTube videos via youtube-transcript-api

Processes transcript text with chunking for better summarization

Summarizes text using Hugging Face's DistilBART summarization model locally (no OpenAI API required)

Simple and interactive UI built with Streamlit for easy input and summary display

Supports multi-language transcript extraction based on YouTube video captions

Prerequisites
Make sure you have the following installed:

Python 3.7 or above

Streamlit

youtube-transcript-api

transformers

torch or tensorflow (for model backend)

python-dotenv (for environment variable management)

Installation
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/yourrepo.git
cd yourrepo
Create and activate a virtual environment (recommended):

bash
Copy
Edit
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Create a .env file in the project root (optional):

You can add any environment variables you need here (e.g., API keys if used later).

Usage
Run the app:

bash
Copy
Edit
streamlit run app.py
Open the URL shown in your browser (usually http://localhost:8501).

Enter the YouTube video URL or video ID.

Click Start to fetch the transcript and generate a summary.

View the summarized content displayed on the page.

Example
Input:
https://www.youtube.com/watch?v=DPmtnb8NBog

Output:
A clear, concise summary of the video transcript with introduction, bullet points, and conclusion.

Notes
The summarization model runs locally, so no API key or billing required.

Transcript availability depends on the video's caption settings.

The model and pipeline use PyTorch or TensorFlow — ensure you have one installed.

Contributing
Feel free to open issues or submit pull requests to improve the app!

License
Distributed under the MIT License. See LICENSE for details.
