# AI-Powered Meeting Assistant

## Overview
The **AI-Powered Meeting Assistant** automates and enhances the meeting documentation process. It transforms raw audio into structured, actionable meeting minutes and tasks, particularly excelling in the complex domain of financial discussions.

## Features
- **Speech-to-Text**: Utilizes **OpenAI Whisper** for highly accurate initial transcription.
- **Transcript Correction**: Uses an **IBM watsonx.ai Large Language Model (Llama-3-2)** to clean the transcript and ensure proper expansion of financial acronyms and terminology.
- **Information Extraction**: A LangChain pipeline processes the cleaned text using a second LLM (**Granite-3**) to intelligently extract:
  - Key Decisions
  - Action Items
  - Meeting Summaries
- **User Interface**: Seamlessly integrated and delivered through a user-friendly **Gradio** web interface.

## Files in the Repository
- `speech2text_app.py`: Gradio web interface for the meeting assistant.
- `speech_analyzer.py`: Main speech analysis script.
- `Requirement.txt`: Project dependencies.
- `sample-meeting.wav`: A sample audio file for testing.

## Getting Started

1. Install dependencies:
   ```bash
   pip install -r Requirement.txt
   ```
2. Run the application:
   ```bash
   python speech2text_app.py
   ```