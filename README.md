# ALX Simple Quiz

A simple interactive quiz application built using HTML, CSS, and JavaScript.  
This project was created by **Mmesoma Chukwumezie** as part of an ALX task to practice DOM manipulation and event handling with vanilla JavaScript.

---

## 📋 Task Description

The goal was to implement JavaScript functionality for a basic quiz.  
Given the HTML and CSS template, the task was to bring the quiz to life by:

- Writing a function to check the selected answer
- Providing feedback to the user
- Handling the submit event correctly

---

## ✅ Features

- Displays a math question with multiple-choice answers
- Validates user’s selected radio option
- Shows dynamic feedback:
  - ✅ "Correct! Well done."
  - ❌ "That's incorrect. Try again!"
- Clean, responsive design

---

## 💡 How It Works

1. The user selects one of the radio button answers.
2. Clicking the **Submit Answer** button triggers the `checkAnswer` function.
3. JavaScript compares the user’s answer to the correct answer (`4`).
4. Feedback is displayed in real-time.

---

## 🧠 Key Concepts Practiced

- DOM selection (`querySelector`, `getElementById`)
- Event handling (`addEventListener`)
- Working with radio buttons
- Conditional logic (`if...else`)

---

## 🔍 Sample JavaScript

```js
function checkAnswer() {
  const correctAnswer = "4";
  const userAnswer = document.querySelector('input[name="quiz"]:checked')?.value;
  const feedback = document.getElementById("feedback");

  if (userAnswer !== correctAnswer) {
    feedback.textContent = "That's incorrect. Try again!";
  } else {
    feedback.textContent = "Correct! Well done.";
  }
}

document.getElementById("submit-answer").addEventListener("click", checkAnswer);

---

## 🔍 How to Run
1. Clone this repository:
 git clone https://github.com/your-username/ALX_Simple_Quiz

2. Open the index.html file in any modern browser.
3. Select an answer and click Submit Answer.

---

## 👩‍💻 Author
Mmesoma Chukwumezie
Aspiring Front-End Developer | Passionate about clean code and meaningful user experiences.

Connect on LinkedIn [www.linkedin.com/in/mmesoma-chukwumezie]

---

## 📄 License

This project is part of the ALX Software Engineering program.
Use it for learning and practice. Attribution appreciated.