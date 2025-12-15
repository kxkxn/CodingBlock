Memory Card Matching Game (Java Swing)
Game Overview

This project is a card-matching memory game built using Java Swing. The game presents a grid of cards that the player flips two at a time in an attempt to find matching pairs.

The board consists of 20 cards, arranged in 5 columns and 4 rows.

Cards are displayed face up for 1.5 seconds at the start of the game, then flipped face down.

The player can flip two cards per turn.

If the two cards match, they remain face up.

If they do not match, they flip back after a short delay.

An error counter tracks the number of incorrect matches.

A Restart Game button allows the player to reshuffle the cards and reset the game state.

Game Logic

Uses a javax.swing.Timer to manage delays when flipping cards back over.

Two variables track the currently selected cards:

cardOneSelected

cardTwoSelected

Card Click Behavior

A card can only be selected if:

The game is ready (no delay in progress)

The card is currently face down

When a card is clicked:

Its image is revealed

If two cards are selected:

Matching cards

Remain face up

Selected card variables are reset

Non-matching cards

Error count is incremented

A 5-second delay occurs

Both cards are flipped face down after the delay

Input Control

User input is disabled during delay periods to prevent additional card selections while cards are being evaluated.

Restart Functionality

The restart button:

Reshuffles the cards

Resets all card states to face down

Clears selected cards

Resets the error counter

Restarts the initial face-up preview timer

Credits

This project is based on a tutorial by Kenny Yip Coding on YouTube.
All credit for the original source code and instructional guidance goes to Kenny Yip.
https://youtu.be/FxDirbh3tXc?si=ev-ISt_lynqNOGY_
