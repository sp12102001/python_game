# Maths Quiz Game -  Python Coursework
The Maths Quiz Game is an interactive, Python-based game developed for the SD1 coursework. It challenges players with a variety of mathematical problems, allowing a head-to-head competition between a human player and the computer, focusing on speed and accuracy in solving math questions.

## Overview

The game offers numerous features, including:

- Difficulty level selection
- Choice of arithmetic operations for practice
- Difficulty adjustment based on player's performance
- Game results displayed through unique ASCII art

## Components

The project comprises several Python scripts:

- **[main.py](http://main.py/):** The central script running the game.
    - **Importing modules:** The script imports essential Python modules and functions from other Python files, like `random`, `time`, and game-specific functions.
    - **ANSI escape codes:** These sequences control the visual appeal of the program's output.
    - **Game banner:** The `get_art` function fetches ASCII art for the game banner.
    - **`computer_play` function:** This function simulates the computer's gameplay using an accuracy threshold and random numbers.
    
    **`adjust_difficulty_based_on_performance` function**
    
    This function alters the game's difficulty level based on the player's performance.
    
    **`display_final_result` function**
    
    This function shows the game's final result using ASCII art.
    
    **`main` function**
    
    This function controls the game's flow. If the player agrees to play, they select the difficulty level and operations, after which the game begins.
    
    **`if __name__ == "__main__": main()`**
    
    This line ensures the `main()` function is called when the script is run directly.
    
    **Other scripts:** The game also uses other Python scripts: `ascii_art.py`, `configurator.py`, `math_question_generator.py`, and `scoring_system.py`. These scripts make the code more structured and manageable.
    
- **ascii_art.py:** This script contains ASCII art displayed during the game.
    - It uses dictionaries to store ASCII art images under the keys: "player_wins", "computer_wins", "tie", and "game_banner". The function `get_art(art_name)` retrieves these images based on the provided key name.
- **[configurator.py](http://configurator.py/):** This script contains functions for choosing the game's difficulty level and arithmetic operations.
    - The `choose_difficulty()` function allows the user to select their preferred question difficulty.
    - The `choose_operations()` function enables users to choose the types of math operations they want to practice.
- **math_question_generator.py:** This script creates the math questions for the quiz.
    - The `generate_math_question` function generates a math question based on a randomly selected operation and difficulty.
    - The `increase_difficulty` function raises the current difficulty level of the questions.
- **scoring_system.py:** This script computes the scores based on the players' answers and response times.
    - The `calculate_score` function compares the correct answer with the player's answer. If the answers match, it calculates a score based on the time taken to answer.
