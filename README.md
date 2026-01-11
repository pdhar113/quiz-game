# Quiz Game

A small command-line quiz game built in Python. Uses a list of question dictionaries in `data.py`, a `Question` model, and a `QuizBrain` controller to run a True/False quiz.

## Requirements

- Python 3.8+

## Quick start

Open a terminal in the project folder and run:

```powershell
python main.py
```

## Project structure

- `main.py` — entry point that wires everything together and starts the quiz.
- `data.py` — question data as a list of dictionaries (`question_data`).
- `question_model.py` — `Question` class representing a single quiz question.
- `quiz_brain.py` — `QuizBrain` class that manages question order, score, and user interaction.

## Notes

- `data.py` contains cleaned, human-readable question text (HTML entities replaced).
- If you hit an `IndexError` related to question list bounds, ensure `QuizBrain.still_has_questions()` correctly checks the list length before calling `next_question()`.

## Contributing

Feel free to add more questions to `data.py` or extend `QuizBrain` to support multiple-choice questions.

## License

MIT — modify as needed.
