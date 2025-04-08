# Interactive Learning Platform 

## 1. Project Purpose

This project is an interactive web-based learning platform designed to present educational content and assess user understanding through quizzes. Initially developed with content focused on the Internet of Things (IoT) and Microcontroller Units (MCU) based on provided lecture materials, the platform is built to be flexible and easily adaptable for different subjects.

The main goal is to provide an engaging and customizable learning experience with features like:
* Dynamic loading of lecture content and corresponding quizzes.
* Multi-lecture selection.
* Interactive multiple-choice quizzes with immediate feedback and explanations.
* User-selectable color themes for visual preference.
* Persistent theme selection using browser storage.
* Responsive design for usability across various devices (desktops, tablets, mobiles).

## 2. Key Features

* **Lecture Selection:** Users can choose from multiple available lectures (currently simulated up to 5).
* **Dynamic Content:** Lecture notes and quiz questions are loaded dynamically (simulated via JavaScript `fetch` from conceptual JSON files).
* **Interactive Quiz:**
    * Multiple-choice questions.
    * Visual feedback upon selecting an answer.
    * Detailed feedback after submitting an answer (highlighting correct/incorrect choices, showing icons).
    * Explanations provided for each question (in Arabic, as per original requirement).
* **Theming:**
    * Multiple pre-defined color themes (10 options).
    * Easy theme switching via a dedicated UI element.
    * Theme preference saved in `localStorage` for persistence.
* **Responsiveness:** The layout adapts to different screen sizes, including handling for wide tables on mobile using horizontal scrolling.
* **User Navigation:** Allows users to navigate back to the current lecture content or the main lecture selection screen from various points (quiz, results).

## 3. Technologies Used

* **Frontend:** HTML5, CSS3, JavaScript (ES6+)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (via Play CDN for rapid prototyping)
* **Icons:** [Font Awesome](https://fontawesome.com/) (via CDN)
* **Fonts:** [Google Fonts](https://fonts.google.com/) (`Inter` for English, `Tajawal` for Arabic)
* **Data Format (Conceptual):** JSON (for structuring lecture and quiz data - currently simulated in JS)
* **Browser APIs:**
    * `fetch` API (Simulated for loading lecture data)
    * `localStorage` API (for saving theme preference)
    * DOM Manipulation

## 4. How to Use / Run

1.  Save the code from the Canvas artifact as an `index.html` file.
2.  (Optional but recommended for full functionality) Create JSON files for each lecture (e.g., `lecture1.json`, `lecture2.json`, ...) following the structure simulated in the JavaScript code. Place these files in the same directory as `index.html` or update the `fetch` paths in the `simulateFetch` function accordingly. *Note: The current version uses simulated data within the script.*
3.  Open the `index.html` file directly in a modern web browser (like Chrome, Firefox, Edge, Safari).
4.  Select a lecture to view the content and start the quiz.
5.  Use the theme switcher (palette icon) in the top-right corner to change the appearance.

## 5. Potential Future Improvements

* Implement actual `fetch` calls to load external JSON files from a server instead of simulating.
* Add more complex question types (e.g., fill-in-the-blanks, matching).
* Track user progress across lectures.
* Implement backend support for user accounts and saving progress centrally.
* Add more sophisticated animations and transitions.
