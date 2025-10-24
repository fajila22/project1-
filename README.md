# Quick Quiz

A lightweight, fully static online quiz you can run by opening `index.html`.

## Features
- **No build or server**: open `index.html` in a browser.
- **Responsive UI** with Tailwind CDN.
- **Categories & difficulty** filters.
- **Timer**: 60s per question, auto-advance.
- **Progress & navigation**: previous/next, clear answer.
- **Scoring and review** with per-question breakdown.
- **Persistence**: quiz state stored in `localStorage` to resume after refresh.

## Files
- `index.html` – UI layout and includes scripts.
- `quizData.js` – Question bank (`QUIZ_QUESTIONS`, `QUIZ_CATEGORIES`).
- `app.js` – Quiz logic.

## Add questions
Edit `quizData.js` and append to the `QUIZ_QUESTIONS` array:
```js
{
  id: 'uniq-id',           // unique string
  category: 'Science',     // any category name
  difficulty: 'easy',      // 'easy' | 'medium' | 'hard'
  type: 'mcq',             // 'mcq' or 'boolean'
  question: 'Your text',
  choices: ['A','B','C','D'], // for boolean, use ['True','False']
  answer: 2                // index into choices (0-based)
}
```

## Run
- Double-click `index.html` (or right-click → Open With → your browser).

## Notes
- To change per-question time, edit `PER_QUESTION_SECONDS` in `app.js`.
- To reset saved progress, click "Clear Saved State" on the results screen.# project 1
- Project Title:
          Online Quiz Application Using Node.js
Objective:
          To design and implement a full-stack web application that allows users to register, attempt quizzes, view results, and track performance — all in a secure, interactive, and user-friendly environment.

Goals:
●	Provide a platform for students to take quizzes online.
●	Allow admin users to create, update, and delete quizzes dynamically.
●	Store and display user performance data with instant feedback.
●	Ensure scalability and secure backend communication through RESTful APIs.

Technology Stack:

Layer	                Technology Used

Frontend	   HTML, CSS, Bootstrap, EJS Templates
Backend	   Node.js with Express.js
Database	   MongoDB (via Mongoose)
Authentication	   JSON Web Token (JWT)
API Testing	   Postman
Deployment	   Render / Vercel / GitHub Pages (frontend)
