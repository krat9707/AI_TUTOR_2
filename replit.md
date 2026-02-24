# AI Tutor - Local AI Study Buddy

## Overview
A Streamlit-based AI tutoring application that provides personalized explanations and generates custom quizzes across multiple subjects. Originally designed to work with Ollama for local AI model inference.

## Project Architecture
- **Framework**: Streamlit (Python)
- **AI Backend**: Ollama (local LLM inference)
- **Config**: YAML-based model configuration in `config/models.yaml`
- **Port**: 5000 (Streamlit frontend)

## Key Files
- `app.py` - Main Streamlit application
- `config/models.yaml` - Model configuration and preferences
- `.streamlit/config.toml` - Streamlit server configuration
- `requirements.txt` - Python dependencies

## Running
The app runs via Streamlit on port 5000:
```
streamlit run app.py
```

## Notes
- The app requires Ollama to be running for AI features to work
- Without Ollama, the UI loads but displays a connection error (handled gracefully)
- Streamlit is configured with CORS and XSRF protection disabled for Replit proxy compatibility
