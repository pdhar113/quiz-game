# Quiz Game 

A fun, interactive True/False quiz game with a GUI built in Python. Test your knowledge across general knowledge, science, entertainment, and more with real-world questions fetched from the Open Trivia Database API.

## Features

✅ **GUI Interface** — Beautiful Tkinter-based user interface with a modern dark theme  
✅ **Real Questions** — Fetches 10 random True/False questions from the Open Trivia Database  
✅ **Instant Feedback** — Canvas background turns green for correct answers, red for incorrect  
✅ **Score Tracking** — Real-time score display throughout the quiz (e.g., Score: 5/10)  
✅ **Final Results** — Summary screen showing your final score at the end  
✅ **HTML Parsing** — Automatically decodes HTML entities in questions for clean display  

## Screenshots

<table>
  <tr>
    <td align="center">
      <img src="images/Screenshot 2026-02-21 155759.png" width="400" alt="Quiz Question Screen">
      <p><strong>Quiz in Progress</strong></p>
    </td>
    <td align="center">
      <img src="images/Screenshot 2026-02-21 155921.png" width="400" alt="Final Score Screen">
      <p><strong>Final Score Screen</strong></p>
    </td>
  </tr>
</table>

## Requirements

- Python 3.8+
- Tkinter (usually included with Python)
- requests library

## Installation

1. Clone or download this project
2. Install required packages:
`ash
pip install requests
`

## Quick Start

Open a terminal in the project folder and run:

`ash
python main.py
`

The quiz window will open automatically. Answer each question by clicking the **True** or **False** button!

## How It Works

1. **Data Fetching** — `data.py` retrieves 10 random True/False questions from the Open Trivia Database API
2. **Question Creation** — `main.py` processes the API response and creates `Question` objects
3. **Quiz Logic** — `quiz_brain.py` manages the quiz flow, scoring, and validation
4. **UI Display** — `ui.py` renders the GUI and handles user interactions with instant visual feedback

## Project Structure

`
quiz-game-start/
├── main.py              # Entry point - initializes the quiz
├── data.py              # Fetches questions from Open Trivia Database API
├── question_model.py    # Question class definition
├── quiz_brain.py        # Quiz logic and score management
├── ui.py                # Tkinter GUI implementation
├── README.md            # This file
└── images/              # UI images (true.png, false.png)
`
