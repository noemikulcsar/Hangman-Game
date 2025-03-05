# Hangman Game Project 🎮

Welcome to the **Hangman** game built using **Java**! This is a simple yet fun word-guessing game that offers different levels of difficulty: **Easy**, **Medium**, and **Hard**.

---

## 🕹️ Game Overview

### Start Page 🏠

- Upon launching the game, the user is presented with 3 difficulty levels:
  - **Easy**
  - **Medium**
  - **Hard**

- When the user selects a difficulty, the game adjusts accordingly and starts a new game.

---

### Game Page 🎮

- The **number of attempts** varies based on the difficulty:
  - Easy: 4 attempts
  - Medium: 6 attempts
  - Hard: 9 attempts
- As the user makes incorrect guesses, the **Hangman figure** is progressively drawn.
- The player inputs **letters** via the keyboard, and the game will validate them against the word being guessed.
- **Hint**: The user can click a "Hint" button to reveal one letter from the word.
- The game ends when:
  - The user guesses the word correctly 🏆
  - The player runs out of attempts 😞
- Users can restart the game at any point.

---

## 🛠️ Components Overview

### 1. **HangmanUI** 🎨
Manages the user interface:
- Displays the start page with difficulty buttons.
- Shows the game progress (attempts left, Hangman figure).
- Contains the **Hint** and **Restart** buttons.
- Updates labels and shows game status (Win/Lose).

### 2. **HangmanGameManager** ⚙️
Handles core game logic:
- Verifies if the player's guess is correct.
- Updates the game status (win/lose).
- Provides hints to the user when requested.

### 3. **HangmanWord** 🔤
- Tracks the word's progress.
- Displays correctly guessed letters and hides unguessed ones.
- Checks if the entire word is guessed.
- Reveals letters when hints are used.

### 4. **HangmanWordGenerator** 💡
Manages the word selection based on difficulty:
- Randomly picks a word from a dictionary for each level.

