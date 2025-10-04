# Astronomy Wordle Game
A fully functional Wordle-style game featuring astronomy terminology, built with Python and powered by Claude AI for hints and educational content.
Overview
This project implements a complete Wordle game using 5-letter astronomy terms. Players have 6 attempts to guess the word, receiving color-coded feedback after each guess:

🟩 GREEN: Letter is correct and in the right position
🟨 YELLOW: Letter is in the word but in the wrong position
⬜ GRAY: Letter is not in the word

The system tracks player statistics, provides AI-generated hints, and offers educational content about each astronomy term after the game concludes.
Features

Multiple Difficulty Levels: Choose from Easy, Medium, Hard, or Mixed difficulty
AI-Powered Hints: Get contextual hints using Claude AI (requires API key)
Educational Content: Learn about each astronomy term after completing a game
Statistics Tracking: Track your wins, streaks, and guess distribution
Visual Statistics: Beautiful matplotlib visualizations of your gameplay stats
Persistent Storage: Game statistics are saved and loaded automatically


Game Structure
Classes

1. WordBank: Manages the collection of astronomy words organized by difficulty

Easy: Common space terms (COMET, ORBIT, VENUS, etc.)
Medium: Standard astronomy vocabulary (DWARF, QUARK, GAMMA, etc.)
Hard: Advanced/obscure terms (BRAHE, METIS, NADIR, etc.)


2. GameState: Manages the current game session

Tracks guesses and remaining attempts
Evaluates guess accuracy with color-coded feedback
Monitors win/loss conditions


3. WordleGame: Main game controller

Orchestrates gameplay flow
Integrates with Claude AI for hints and education
Manages statistics and visualization



How to Play

Run the Jupyter notebook or Python script
Enter your Anthropic API key when prompted (optional - game works without it)
Choose your difficulty level (1-4)
Enter 5-letter guesses
Type 'hint' for an AI-generated clue
Type 'quit' to exit
View your statistics after each game

Statistics
The game tracks:

Games played and won
Win rate percentage
Current and maximum win streaks
Distribution of guesses needed to win
Average number of guesses

Statistics are visualized with:

Bar chart showing guess distribution
Summary panel with key statistics
Saved as wordle_statistics.png

API Integration
The game uses Claude AI (Anthropic) for:

Hints: Context-aware clues that don't give away the answer
Educational Content: Detailed explanations of astronomy terms

Note: The game is fully playable without an API key, but hints and educational content will be limited.

Author
Evan Stiverson

GitHub: Evan-Stiverson
Repository: Astro_Data_Project_1

License
This project is open source and available for educational purposes.
