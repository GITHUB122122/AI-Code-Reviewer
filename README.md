# AI Code Reviewer

An AI-powered code review application that analyzes submitted code and provides intelligent feedback using Google's Gemini API.

## Overview

AI Code Reviewer is a web application built to help developers improve their code quality. Users can submit code through a simple interface and receive AI-generated reviews highlighting potential issues and suggesting improvements.

The application uses React for the frontend and Node.js with Express for the backend, keeping the user interface and AI processing logic separate.

## Features

- **AI-Powered Code Reviews:** Uses Google's Gemini API to analyze submitted code.
- **Code Quality Analysis:** Evaluates readability, maintainability, and coding practices.
- **Bug Detection:** Identifies potential logical errors and coding issues.
- **Performance Suggestions:** Highlights opportunities for optimization.
- **Security Awareness:** Looks for common security vulnerabilities.
- **Improvement Suggestions:** Provides recommendations and improved code examples.

## Tech Stack

**Frontend**
- React.js
- Vite
- JavaScript
- CSS

**Backend**
- Node.js
- Express.js
- Google Gemini API
- dotenv
- Axios / CORS

## Project Structure

```text
AI-Code-Reviewer/
│
├── BackEnd/
│   ├── src/
│   │   ├── controllers/
│   │   ├── routes/
│   │   └── services/
│   ├── server.js
│   ├── package.json
│   └── package-lock.json
│
├── Frontend/
│   ├── public/
│   ├── src/
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
│
├── .gitignore
└── README.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/GITHUB_USERNAME/AI-Code-Reviewer.git
```

### 2. Install frontend dependencies

```bash
cd AI-Code-Reviewer/Frontend
npm install
```

### 3. Install backend dependencies

Open another terminal:

```bash
cd AI-Code-Reviewer/BackEnd
npm install
```

### 4. Configure environment variables

Create a `.env` file inside the `BackEnd` directory.

Add your Gemini API key:

```env
GOOGLE_GEMINI_KEY=your_gemini_api_key
```

Get your API key from [Google AI Studio](https://aistudio.google.com/apikey).

### 5. Start the backend

Inside the BackEnd directory:

```bash
node server.js
```

The backend runs at:

`http://localhost:3000`

### 6. Start the frontend

Inside the Frontend directory:

```bash
npm run dev
```

Open the local URL provided by Vite, usually:

`http://localhost:5173`

## API Endpoint

| Method | Endpoint | Description |
|---|---|---|
| POST | `/ai/get-review` | Submits code for AI review |

## Environment Variables

| Variable | Description |
|---|---|
| `GOOGLE_GEMINI_KEY` | Google Gemini API key |

## Future Improvements

- Support for multiple programming languages.
- Improved error handling and API response management.
- Review history and saved code reviews.
- More detailed code analysis and recommendations.
- Deployment with a publicly accessible interface.

## Author

Developed as a project to explore AI integration, full-stack development, and practical applications of Large Language Models.

---

**Note:** Gemini API usage is subject to Google's model availability, rate limits, and usage policies.
