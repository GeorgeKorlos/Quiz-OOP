This repository contains a simple command-line quiz game built in Python. The game quizzes users with true/false questions and keeps track of their score.

data.py
This file contains the data for the quiz in the form of a list of dictionaries. Each dictionary contains a question (as text) and its corresponding answer (as answer).

main.py
This is the main script that initializes the quiz game. It imports the questions from data.py, creates instances of the Question class, and adds them to the QuizBrain. It then runs the quiz in a loop until all questions have been answered, and finally prints the user's score.

question_model.py
This file defines the Question class, which represents a single question in the quiz. Each Question object has two attributes: the question text and the correct answer.

quiz_brain.py
This file contains the QuizBrain class, which manages the quiz process. It tracks the current question number, checks if there are more questions to ask, retrieves the next question, and checks the user's answer against the correct answer.

Key methods:

still_has_questions(): Returns True if there are more questions in the list.
next_question(): Retrieves the next question and prompts the user for their answer.
check_answer(): Compares the user's answer with the correct answer and updates the score accordingly.
