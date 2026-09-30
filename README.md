# EduGenie: Google Gemini Powered Learning Assistant

An intermediate-level educational web application that uses the Google Gemini API
to provide explanations, examples, and AI-generated practice quizzes.

## Features

- AI learning chat
- Topic explanations
- Simple examples and step-by-step help
- AI-generated MCQ quizzes
- Responsive web interface
- Gemini API integration through a Flask backend
- API key kept on the server in `.env`

## Technology Stack

- Python
- Flask
- Google GenAI Python SDK
- Google Gemini API
- HTML5 / CSS3 / JavaScript

## Project Structure

```text
EduGenie_Project/
├── app.py
├── requirements.txt
├── .env.example
├── .gitignore
├── README.md
├── templates/
│   └── index.html
└── static/
    ├── style.css
    └── app.js
```

## Setup

1. Install Python 3.10+.
2. Open a terminal in this project folder.
3. Create a virtual environment:

```bash
python -m venv .venv
```

4. Activate it.

Windows:
```bash
.venv\Scripts\activate
```

macOS/Linux:
```bash
source .venv/bin/activate
```

5. Install packages:

```bash
pip install -r requirements.txt
```

6. Copy `.env.example` to `.env`.
7. Put your Gemini API key in `.env`.
8. Start the app:

```bash
python app.py
```

9. Open:

```text
http://127.0.0.1:5000
```

## Getting a Gemini API key

Use Google AI Studio's API Keys page. Keep the key private and never commit
`.env` to GitHub.

## GitHub

Create a new GitHub repository, then upload all project files. Do not upload
`.env`.

Typical commands:

```bash
git init
git add .
git commit -m "Initial EduGenie project"
git branch -M main
git remote add origin YOUR_GITHUB_REPOSITORY_URL
git push -u origin main
```

## Important

The frontend does not contain the Gemini API key. Requests go to Flask,
and Flask calls Gemini. This is safer than putting the API key in browser
JavaScript.

## Academic Project Description

**Title:** EduGenie: Google Gemini Powered Learning Assistant

**Objective:** To develop an AI-based learning assistant that helps students
understand academic topics, ask questions, receive explanations, and practice
with automatically generated quizzes.

**Modules:**
1. User Interface
2. AI Chat Module
3. Quiz Generator
4. Gemini API Integration
5. Error Handling
6. Responsive Web Design

**Future Enhancements:**
- Student login
- Progress tracking
- SQLite database
- PDF/document question answering
- Voice input
- Teacher dashboard
- Study-plan generation
