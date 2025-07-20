
# 🎲 Dice-Game

## Overview

This repository contains the **Dice Game**, a two-player dice game implemented using **HTML**, **CSS**, and **JavaScript**.
Players compete to reach a total score of **100 points** by strategically rolling a die and banking points—while risking their current score if they roll a 1.
The game features a clean, interactive UI with visual feedback for the active player and winner, including animations for an engaging experience.

## 🎯 Game Rules

### Objective

* Be the first player to reach a total score of **100 points**.

### Gameplay

* Players take turns rolling a single die.
* Each roll (2–6) adds the die's value to the player's current score.
* Rolling a **1** resets the player's current score to 0 and switches the turn to the other player.
* Players can choose to **Hold**, adding their current score to their total score, then passing the turn.

### Winning

* The first player to reach or exceed **100 points** wins.
* The winner's section is **highlighted** and **scaled up** for emphasis.

### New Game

* The **"New Game"** button resets all scores and starts a fresh game.

## ✨ Features

* Interactive and responsive UI with distinct player sections showing names and scores.
* Dynamic die display that updates with the rolled value (1–6) and hides when not in use.
* Visual feedback:

  * Active player's section is highlighted via the `.player--active` class.
  * Winner's section is styled with a **dark gray background (#2f2f2f)** and scaled up **1.5x** using `transform: scale(1.5)` with a **1.5-second transition**.
* Robust game state management for tracking scores, active player, and game status.
* Reset functionality to start a new game with cleared scores and initial state.

## 🛠 Technical Details

### HTML

* Structured with:

  * Player sections: `.player--0`, `.player--1`
  * Score displays: `#score--0`, `#score--1`, `#current--0`, `#current--1`
  * Die image: `.dice`
  * Buttons: "Roll Dice", "Hold", "New Game"

### CSS

* Styles the layout, player sections, and die.
* Applies `.player--winner` styling:

  * Dark gray background
  * 1.5x scaling
  * Smooth transition

### JavaScript

* Handles game logic:

  * Random die rolls
  * Score updates
  * Player switching
  * Win detection
* Manages DOM updates for:

  * Scores
  * Die images
  * Player states
* Implements event listeners for:

  * "Roll Dice"
  * "Hold"
  * "New Game"
* Tracks:

  * `activePlayer`
  * `currentScore`
  * `scores` (array for total scores)
  * `playing` (game state)

## ⚙️ Setup

* Clone the repository and open `index.html` in a browser.
* Ensure `dice1.png` to `dice6.png` images are in the correct directory.
* Link `styles.css` and `script.js` in `index.html`.
* No external dependencies required; runs in any modern browser.

## 🚀 Usage

* Click **"Roll Dice"** to roll the die and add to the current score.
* Click **"Hold"** to bank the current score into the total score.
* Avoid rolling a **1**, which resets the current score and switches players.
* First to **100 points** wins, with their section scaled up and highlighted.
* Click **"New Game"** to reset and start over.

## 🔮 Future Enhancements

* Add **sound effects** for rolls, holds, and winning.
* Allow **customizable winning scores** via an input field.
* Implement a **mobile-friendly layout** with touch controls.
* Add **player name input** for personalization.

---

This repository offers a fun and educational implementation of the **Pig Game**, perfect for learning:

* JavaScript DOM manipulation
* Event handling
* CSS animations
