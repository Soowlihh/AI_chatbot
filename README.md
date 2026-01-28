# AI Chatbot (FastAPI)

## Overview
A FastAPI-based chatbot backend that routes user messages to an LLM provider and returns responses via a REST API. Built to practice API design, secure config handling, and deployable backend structure.

## Tech Stack
- Python, FastAPI
- REST API
- Environment-based config (no secrets committed)
- (Optional: Docker / CI/CD if you have it)

## Features
- Chat endpoint that accepts user input and returns model responses
- Simple agent/router layer for response generation
- Configurable model provider via environment variables

## Setup (Local)
```bash
python -m venv .venv
source .venv/bin/activate   # (Windows: .venv\Scripts\activate)
pip install -r requirements.txt
cp API.env.example API.env
uvicorn app:app --reload


