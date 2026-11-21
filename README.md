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

```bash


Tata Stanley Mbajing
Junior FrontEnd Developer
[📩 Email: (stanleymbajingtata@gmail.com)]
🌍 Based in Cameroon | Open to remote opportunities
