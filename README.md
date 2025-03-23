# YouTube-Transcript-Summarizer
YouTube Transcript Summarizer is a Python-based tool that extracts and summarizes YouTube video transcripts using TF-IDF. It automates transcript retrieval via youtube_transcript_api and employs scikit-learn for extractive summarization.

Overview:-
This project extracts and summarizes the transcript of a given YouTube video. It uses the youtube_transcript_api library to fetch the transcript, and sklearn's TfidfVectorizer to perform extractive summarization.

Features:-
Fetches YouTube video transcripts automatically.
Performs extractive summarization using TF-IDF.
Configurable compression ratio for summary length.
Handles missing transcripts and short videos gracefully.

Installation:-
Ensure you have Python installed (>=3.7). Install the required dependencies:
pip install youtube-transcript-api scikit-learn nltk numpy

Libraries Used:-
youtube_transcript_api: Fetches YouTube video transcripts without requiring YouTube API keys.
scikit-learn (sklearn): Provides TfidfVectorizer for feature extraction and text representation.
nltk (Natural Language Toolkit): Used for sentence tokenization.
numpy: Used for numerical computations, specifically handling TF-IDF scores.

How It Works
Fetching Transcripts:
The get_video_transcript function extracts subtitles from a given YouTube video using youtube_transcript_api.
It joins all subtitle segments into a single string.

Summarization Process:
The text is split into sentences using sent_tokenize from NLTK.
The TfidfVectorizer is used to compute the importance of each sentence.
Sentences with the highest scores are selected for the summary.

















