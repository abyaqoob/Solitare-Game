♠️ Solitaire Game in C++

📘 Project Overview

This is a console-based implementation of the Solitaire card game, developed in C++ as a Data Structures course project. The game is built from scratch without using the STL (Standard Template Library) and emphasizes the application of core data structures to model card movements and game logic.

🧠 Learning Objectives

This project was designed to strengthen understanding of the following data structures and programming concepts:

Doubly Linked Lists: Used for card storage in tableau columns and the main deck.
Stacks: Used to manage the stock, waste, and foundation piles.
Custom Iterators: Implemented to traverse custom list structures.
Undo Stack: Enables players to reverse previous moves using a command stack.
Object-Oriented Programming: Applied throughout the design using classes for Card, Game, Command, Stack, and List.

🎮 Game Features

Full Solitaire game logic with:
Drawing from stock to waste
Moving cards between tableau columns
Moving cards to/from foundation piles
Moving cards from waste to tableau/foundation
Undo functionality for supported actions
Unicode suit display using wcout and console coloring
Hidden and revealed card states
Game-win detection when all foundation piles are complete
🗂️ Main Classes and Structures

Card: Stores card suit, rank, visibility, and color logic.
List<T>: Custom doubly linked list implementation with iterators.
Stack<T>: Stack implementation using the custom linked list.
Game: Central class handling the deck, tableau, stock, waste, foundations, and game rules.
Command: Stores move history for the undo feature.
🛠️ How to Run

Open the project in Visual Studio (with support for wide characters and ANSI color codes).
Compile the code.
Run the program.
Use the console to input commands in the following formats:
s — Draw from stockpile
m c1 c2 n — Move n cards from column c1 to column c2
m c1 f1 1 — Move a card from column c1 to foundation f1
m w f1 1 — Move a card from waste to foundation f1
m w c1 1 — Move a card from waste to column c1
m f1 c1 1 — Move a card from foundation f1 to column c1
z — Undo the last move
