# 🎮 Guess the Number — Weekend Edition

A command-line number guessing game built with Bash. The Weekend Edition extends the original Day 3 implementation with multiple difficulty levels, player statistics, personal best tracking, and a leaderboard.

## 📌 Project Overview

Guess the Number is an interactive Bash game where players try to identify a randomly generated number within a specified range.

Players can choose a difficulty level, track their previous games, compete for the best scores, and manage their personal game history.

## ✨ Features

- **Player Name Validation:** Accepts names containing 1–20 letters, digits, or underscores.
- **Multiple Difficulty Levels:** Choose between Easy, Normal, and Hard.
- **Interactive Gameplay:** Receive hints indicating whether your guess is too high or too low.
- **Game Cancellation:** Enter `q` to cancel a game and return to the main menu.
- **Game History:** View previous games, including difficulty, attempts, completion time, and date.
- **Personal Best:** Automatically compares your performance with previous games on the same difficulty.
- **Leaderboard:** Displays the top five players for the selected difficulty.
- **Score Validation:** Detects damaged score records, skips invalid entries, and displays a warning.
- **History Management:** Delete your personal game history with confirmation.
- **Game Statistics:** View total games played and average attempts across all difficulty levels.

## 🎯 Difficulty Levels

| Difficulty | Number Range |
| --- | --- |
| Easy | 1–50 |
| Normal | 1–100 |
| Hard | 1–1000 |

Normal is the default difficulty when no level is specified.

Difficulty names are case-insensitive.

## 🛠️ Requirements

- Linux or another Unix-like operating system.
- Bash shell.
- Standard command-line utilities such as `date`, `awk`, `sort`, and `mktemp`.

## 🚀 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/stanlee21/bash-05-guess-game.git
```

### 2. Navigate into the project directory

```bash
cd bash-05-guess-game
```

### 3. Make the script executable

```bash
chmod +x guess-game.sh
```

### 4. Start playing

Run the game using your player name and an optional difficulty level:

```bash
./guess-game.sh Ama easy
```

You can also start with the default Normal difficulty:

```bash
./guess-game.sh Ama
```

The player name is automatically converted to lowercase.

## 🎮 How to Play

After starting the game, you will see the main menu:

1. **Play:** Start a new guessing game. Enter a number within the selected difficulty range. The game provides hints until you guess correctly. Enter `q` to cancel.
2. **My History:** View your previous completed games and statistics.
3. **Leaderboard:** View the top five players for the selected difficulty.
4. **Delete My History:** Delete your personal game records after confirmation.
5. **Quit:** Exit the game.

## 📁 Game Data Format

The game stores its records in `score.txt` by default.

Each completed game is stored as a pipe-separated record containing:

```text
player|difficulty|attempts|duration|date
```

Example:

```text
ama|easy|6|24|2026-11-23
```

The fields represent:

- `player`: The player's name.
- `difficulty`: The selected difficulty level.
- `attempts`: Number of valid guesses used.
- `duration`: Time taken to complete the game, in seconds.
- `date`: Date the game was completed.

The game file can be changed using the `GAMES_FILE` environment variable:

```bash
GAMES_FILE=test.txt ./guess-game.sh Ama easy
```

When `GAMES_FILE` is not set, the game uses `score.txt`.

## 🧪 Testing

Run the game with different player names and difficulty levels. Test invalid inputs, game cancellation, history, leaderboard, and history deletion.

To check the script for common Bash issues, run:

```bash
shellcheck guess-game.sh
```

## 👨‍💻 Author

Tata Stanley Mbajing
