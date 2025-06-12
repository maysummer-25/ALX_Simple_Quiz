# ALX Simple Projects by Mmesoma Chukwumezie

This repository contains two beginner-friendly JavaScript projects completed as part of the ALX Software Engineering training. The projects helped reinforce my understanding of JavaScript fundamentals by adding interactivity to static HTML pages.

---

## 📘 1. Simple Interactive Quiz

### ✅ Description

A minimal quiz app that checks the user's answer to a single question and provides instant feedback. This project introduced me to event handling, DOM manipulation, and conditional logic in JavaScript.

### 🧠 Features

- Displays a multiple-choice question: *What is 2 + 2?*
- Allows the user to select one answer.
- On clicking **Submit Answer**, the app checks correctness and displays:
  - ✅ "Correct! Well done." if the answer is correct.
  - ❌ "That's incorrect. Try again!" if wrong.

### 🛠 Technologies

- HTML
- CSS
- JavaScript

### 📂 Files

- `index.html`: Markup for the quiz structure.
- `styles.css`: Styling for the quiz.
- `quiz.js`: JavaScript logic that checks the answer.

### 🔍 How It Works

The `checkAnswer()` function:
- Retrieves the selected radio input.
- Compares the value to the correct answer (`"4"`).
- Updates the feedback text based on the result.

---

## 📘 2. Simple Calculator

### ✅ Description

An interactive calculator app that performs basic arithmetic operations (addition, subtraction, multiplication, division). This task helped me understand functions, input handling, and event-driven programming.

### 🧠 Features

- Two number input fields
- Four operation buttons: `+`, `-`, `*`, `/`
- Displays the result after each calculation

### 🛠 Technologies

- HTML
- CSS
- JavaScript

### 📂 Files

- `calculator.html`: Layout and buttons
- `calculator.css`: Styles for inputs and buttons
- `calculator.js`: Logic to perform calculations and handle user input

### 🔍 How It Works

- Each operation has its own function: `add()`, `subtract()`, `multiply()`, `divide()`.
- `parseFloat()` converts string inputs to numbers.
- If input is empty, `|| 0` ensures the value defaults to 0.
- Results are shown dynamically using DOM manipulation.

### 📝 Example:

```js
function add(num1, num2) {
  return num1 + num2;
}
document.getElementById("add").addEventListener("click", function () {
  const number1 = parseFloat(document.getElementById("number1").value) || 0;
  const number2 = parseFloat(document.getElementById("number2").value) || 0;
  const result = add(number1, number2);
  document.getElementById("calculation-result").textContent = result;
});

```

## 🎯 What I Learned
How to manipulate the DOM using JavaScript

Handling user events like click

Using parseFloat() and || for safe input parsing

Separating logic (JavaScript) from structure (HTML) and style (CSS)

Writing modular and readable functions for better code reuse

---

## 🔗 Repository Structure

ALX_Simple_Quiz/
│
├── index.html         # Quiz app
├── styles.css         # Styles for quiz
├── quiz.js            # Quiz logic
│
├── calculator.html    # Calculator UI
├── calculator.css     # Calculator styling
└── calculator.js      # Calculator logic

---

## 🧑‍💻 Author
Mmesoma Chukwumezie
Aspiring Front-End Developer | Passionate about creating interactive web experiences.