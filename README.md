# YouTube Video Summarizer

A Python Streamlit web app that summarizes YouTube video content by extracting the transcript and generating a concise summary using a local Hugging Face transformer model.

Features:
Extracts transcripts directly from YouTube videos via youtube-transcript-api,
Processes transcript text with chunking for better summarization,
Summarizes text using Hugging Face's DistilBART summarization model locally (no OpenAI API required),
Simple and interactive UI built with Streamlit for easy input and summary display,
Supports multi-language transcript extraction based on YouTube video captions.

Prerequisites
Make sure you have the following installed:

Python 3.7 or above,
Streamlit,
youtube-transcript-api,
transformers,
torch or tensorflow (for model backend),
python-dotenv (for environment variable management).

usage 

run streamlit python run...
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
