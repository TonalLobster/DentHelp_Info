# DentHelp - Dental Assistant AI

## Overview
DentHelp is an AI-powered dental assistant application designed to streamline clinical workflows by automating the transcription and summarization of dental appointments. Leveraging advanced speech recognition and natural language processing (NLP), DentHelp processes audio recordings from dental consultations, removes silent segments, transcribes spoken content into text, and generates concise summaries focused on patient condition, diagnosis, treatment plans, and key notes. 
The backend is built with Python and integrates with Google Cloud's Speech-to-Text and Vertex AI services, while the frontend is developed using Bubble, a no-code platform for rapid UI prototyping and database management.


This project aims to replace the manual note-taking duties of a dental assistant, enhancing efficiency and reducing operational costs for dental practices, particularly in Swedish-speaking environments.


# Features
#### Voice Activity Detection (VAD): 
Utilizes librosa to identify and remove silent intervals from audio recordings, optimizing processing time and reducing API costs.

#### Speech-to-Text Transcription: 
Employs Google Cloud Speech-to-Text API for accurate transcription of Swedish-language audio into text.

#### Text Summarization: 
Leverages Vertex AI's text-bison model to generate structured summaries of dental appointments, focusing on critical medical details.

#### RESTful API: 
Built with Flask, providing a lightweight and scalable endpoint for audio processing and summary generation.

#### No-Code Frontend: 
Integrates with Bubble for an intuitive user interface and database storage of summaries.

#### GDPR Compliance: 
Implements HTTPS for secure data transmission and ensures user consent for processing sensitive patient data.


# Technology Stack
## Backend
#### Python 3.9: 
Core programming language for the application logic.

#### Flask: 
Micro web framework for building the RESTful API.

#### Google 
Cloud Speech-to-Text: Real-time audio transcription with Swedish language support.

#### Google Cloud Vertex AI: 
Text generation and summarization using the text-bison model.

#### Librosa: 
Audio processing library for voice activity detection.

#### Soundfile: 
Handles audio file I/O and format conversion.


## Frontend
##### Bubble: 
No-code platform for UI design and database management.


## Deployment
#### Google Cloud Run: 
Serverless platform for deploying the Flask application.

#### Docker: 
Containerization for consistent runtime environments.
