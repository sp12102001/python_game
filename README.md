# Maths Quiz Game - SD1 Python Coursework

The Maths Quiz Game is an interactive, Python-based game developed for the SD1 coursework. It challenges players with a variety of mathematical problems, allowing a head-to-head competition between a human player and the computer, focusing on speed and accuracy in solving math questions.

## Introduction

Designed to be both educational and entertaining, this game aims to enhance mathematical skills through a fun and competitive format. Players can choose their difficulty level and the types of operations they want to focus on, making it a customizable learning experience.

## Modules and Scripts Breakdown

### `random`

This module is essential for the dynamic nature of the game. It generates random numbers that form the basis of the math questions posed to the players. Additionally, it simulates the computer's accuracy in answering questions, adding an element of unpredictability to the game.

### `time`

Time tracking is crucial for adding a competitive edge to the game. This module measures how long it takes for a player to answer each question, influencing the scoring system based on speed and efficiency.

### `math_question_generator`

Contains two key functions:
- `generate_math_question(difficulty_level, operations)`: Creates random math questions based on the selected difficulty level and operation types. It ensures a varied and challenging experience for the player.
- `increase_difficulty(current_difficulty)`: A mechanism to increase the game's difficulty as the player progresses, ensuring that the game remains challenging and engaging.

### `scoring_system`

Features the `calculate_score(correct_answer, player_answer, time_taken)` function. It computes the player's score for each question, taking into account the correctness of the answer and the time taken to provide it. This encourages not only accuracy but also promptness in responses.

### `configurator`

Houses two functions for game customization:
- `choose_difficulty()`: Allows players to select the game's difficulty level, tailoring the challenge to their comfort level.
- `choose_operations()`: Lets players choose the types of math operations (addition, subtraction, multiplication, division) they want to be tested on, allowing for focused practice on specific areas.

### `ascii_art`

Utilizes `get_art(art_name)`: Fetches and displays ASCII art for different game states (e.g., game start, player wins, computer wins). This adds a visual appeal and enhances the user experience.

## ANSI Escape Codes

To make the game visually engaging, ANSI escape codes are used throughout the console output for adding color and style. This includes:
- Different colors for various messages (e.g., cyan for welcome messages, green for correct answers, red for incorrect answers).
- Text styles such as bold and flashing to highlight important game events and achievements.

## Game Flow

1. **Start**: Displays a colorful banner and welcomes the player.
2. **Configuration**: Players set their preferred difficulty level and math operation types.
3. **Gameplay**: Involves a continuous loop where:
   - Questions are generated and presented.
   - The computer 'plays' by randomly determining its success.
   - Players input their answers.
   - Scores are calculated based on response correctness and speed.
   - Difficulty adjustments are made based on player performance.
4. **Conclusion**: Ends with a display of final scores and an outcome message (player win, computer win, or tie).

## Key Functions Explained

- `computer_play(difficulty_level)`: Simulates the computer's attempt at answering questions, with the success rate influenced by the difficulty level.
- `adjust_difficulty_based_on_performance(...)`: Adjusts the game's difficulty based on the comparative scores of the player and computer, ensuring a balanced and fair challenge.
- `display_final_result(...)`: Concludes the game by displaying ASCII art that reflects the outcome, celebrating the player's win, acknowledging the computer's win, or declaring a tie.

## Running the Game

Execute the `main()` function to start the game. Follow the prompts to configure your game settings and begin the challenge. Answer as many questions as you can, as accurately and quickly as possible, to score higher than the computer.

### Conclusion

The Maths Quiz Game is designed to be an engaging way to practice and improve mathematical skills. With its customizable difficulty and operation types, it caters to learners at various levels, providing a challenging yet fun experience. Dive in and test your math prowess against the computer today!
