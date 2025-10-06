# FINWISE
# FINWISE – Finance Chatbot

AI-powered personal finance assistant with calculators, learning tasks, and a chat interface.

## Features
- Chatbot for general finance guidance (with disclaimers)
- Savings Goal Calculator (`Savings_Goal_Calculator.html`)
- Returns Estimator (`Returns_Estimator.html`)
- Credit Score Estimator (`Credit_Score_Estimator.html`)
- Quiz (`quiz.html`)
- Tasks page with curated YouTube learning tasks (`NEWS.html`)
- Retro-styled `homepage.html` linking to all tools

## Run Locally
1) Install
```
npm install
```
2) Start
```
npm start
```
3) Open
```
http://localhost:5000/
```

## Environment (optional)
Set your Gemini key if available (PowerShell):
```
$env:GOOGLE_API_KEY="YOUR_GEMINI_API_KEY(ADD IN SEREVER.JS ON LINE 33)"; npm start
```
Chat gracefully falls back to helpful guidance if live model access isn’t available.

## API
- `GET /health` → service status
- `POST /chat` body: `{ "message": "your question" }`

## Project Structure
- `server.js` – Express server, chat endpoint, static serving
- `homepage.html` – Landing + navigation
- `chat.html` – Chat UI hitting `/chat`
- Tools: `Returns_Estimator.html`, `Savings_Goal_Calculator.html`, `Credit_Score_Estimator.html`, `quiz.html`, `NEWS.html`

## Author
DHVANISH DHULLA
