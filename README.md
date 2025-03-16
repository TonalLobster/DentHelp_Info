# DentHelp - Dental Assistant AI

## Overview
DentHelp is an AI-powered dental assistant application designed to streamline clinical workflows by automating the transcription and summarization of dental appointments. Leveraging advanced speech recognition and natural language processing (NLP), DentHelp processes audio recordings from dental consultations by removing silent segments, transcribing spoken content into text, and generating concise summaries focused on patient condition, diagnosis, treatment plans, and key notes.  
The backend is built with Python and integrates with OpenAI’s APIs (Whisper for transcription and ChatGPT for summarization), while the frontend is developed using Bubble, a no-code platform for rapid UI prototyping and database management.

This project aims to replace the manual note-taking duties of a dental assistant, enhancing efficiency and reducing operational costs for dental practices, particularly in Swedish-speaking environments.

## Features
#### Voice Activity Detection (VAD): 
Utilizes librosa to identify and remove silent intervals from audio recordings, optimizing processing time and reducing API costs.

#### Speech-to-Text Transcription: 
Employs OpenAI's Whisper API for accurate transcription of Swedish-language audio into text.

#### Text Summarization: 
Leverages OpenAI's ChatGPT (or GPT-3.5-turbo) API to generate structured summaries of dental appointments, focusing on critical medical details.

#### RESTful API: 
Built with Flask, providing a lightweight and scalable endpoint for audio processing and summary generation.

#### No-Code Frontend: 
Integrates with Bubble for an intuitive user interface and database storage of summaries.

#### GDPR Compliance: 
Implements HTTPS for secure data transmission and ensures user consent for processing sensitive patient data.

## Technology Stack

### Backend
- **Python 3.9 (or later):** Core programming language for the application logic.
- **Flask:** Micro web framework for building the RESTful API.
- **OpenAI API:**  
  - **Whisper:** For real-time audio transcription with Swedish language support.  
  - **ChatGPT / GPT-3.5-turbo:** For generating structured text summaries of dental consultations.
- **Librosa:** Audio processing library for voice activity detection.
- **Soundfile, Pydub & Torchaudio:** Handles audio file I/O, format conversion, and audio processing.

### Frontend
- **Bubble:** No-code platform for UI design and database management.

## Deployment
- **Google Cloud Run:** Serverless platform for deploying the Flask application.
- **Docker:** Containerization for consistent runtime environments.
