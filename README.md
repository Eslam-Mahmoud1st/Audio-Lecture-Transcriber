# Audio Lecture Transcriber & Notes Generator 

A local Python CLI utility designed for students and self-learners to convert recorded audio and video lectures into clean, structured text notes (`.docx`). Built entirely with Python and powered by OpenAI's open-source Whisper model for fast, accurate, offline speech recognition.

---

## Key Features

- Offline & Private All transcription runs locally on your machine—no cloud APIs, subscriptions, or data sharing required.
- Multi-Format Support Processes both audio (`.mp3`, `.wav`, `.m4a`) and video (`.mp4`, `.mkv`) formats seamlessly.
- Multilingual Support Supports English, Arabic, and multiple other languages automatically.
- Word Document Export Automatically generates formatted Word documents (`.docx`) containing the transcribed notes.
- Memory Efficient Processes media in-memory using arrays to bypass system dependency issues on Windows.

---

## Tech Stack

- Python 3.x
- [openai-whisper](httpsgithub.comopenaiwhisper) Local Automatic Speech Recognition (ASR).
- [python-docx](httpspython-docx.readthedocs.io) Document creation and structure.
- [MoviePy](httpszulko.github.iomoviepy) Media processing and audio extraction.
- [SciPy](httpsscipy.org) Audio signal processing and memory array extraction.

---

## Installation & Setup

1. Clone the repository
   ```bash
   git clone [httpsgithub.comYOUR_USERNAMEaudio-lecture-transcriber.git](httpsgithub.comYOUR_USERNAMEaudio-lecture-transcriber.git)
   cd audio-lecture-transcriber

  Install dependencies
   pip install openai-whisper python-docx moviepy scipy soundfile numpy

Usage
  Run the script
   python transcriber.py

  Enter the path to your audio or video file when prompted
   Enter path to audiovideo file (e.g. lecture.mp4, audio.mp3) lecture.mp4

  The script will output a preview in the terminal and save the full transcription as a .docx file in the same directory!