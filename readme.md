# 🧠 Quick Quiz

A **lightweight, fully static online quiz** you can run by simply opening `index.html` in your browser.  
No servers, no build tools — just pure HTML, CSS (Tailwind), and JavaScript. 🚀  

---

## 🌟 Features

- **No build or server** – open `index.html` directly in any modern browser.  
- **Responsive UI** – clean and mobile-friendly, powered by Tailwind CSS CDN.  
- **Categories & difficulty filters** – choose quiz topics and levels.  
- **Timer** – 60 seconds per question (auto-advances when time runs out).  
- **Progress & navigation** – Previous / Next / Clear Answer buttons.  
- **Scoring & review** – final breakdown with your answers vs correct ones.  
- **Persistence** – quiz state is saved in `localStorage`, so you can refresh or close the tab and resume later.  

---

## 🧩 Project Files

| File | Description |
|------|--------------|
| `index.html` | Main layout and UI, includes scripts and Tailwind CSS. |
| `quizData.js` | Contains question bank (`QUIZ_QUESTIONS`, `QUIZ_CATEGORIES`). |
| `app.js` | Core quiz logic: navigation, timer, scoring, persistence. |

---

## 🧠 How to Add Questions

Edit **`quizData.js`** and append a new object to the `QUIZ_QUESTIONS` array:

```js
{
  id: 'uniq-id',            // unique string ID
  category: 'Science',      // any category name
  difficulty: 'easy',       // 'easy' | 'medium' | 'hard'
  type: 'mcq',              // 'mcq' or 'boolean'
  question: 'Your question text',
  choices: ['A', 'B', 'C', 'D'], // for boolean use ['true', 'false']
  answer: 2                 // index of correct answer (0-based)
}
