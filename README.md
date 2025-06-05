♠️ Solitaire Game – Data Structures Project (C++)

📘 Project Overview

This project is a console-based version of Solitaire, developed in C++ for a Data Structures course. The game simulates core Solitaire mechanics while emphasizing the implementation and use of fundamental data structures without relying on the Standard Template Library (STL).

It served as a learning platform to apply Object-Oriented Programming (OOP) and understand the real-world application of data structures in game development.

<br>
🧠 What I Learned

This project deepened my understanding of:

✅ Doubly Linked Lists – Used for managing columns (tableau) and the deck.
✅ Stacks – Used for the stockpile, wastepile, and foundation piles.
✅ Custom Iterators – Created to traverse custom data structures efficiently.
✅ Undo Mechanism – Stack of Command objects enables undo functionality.
✅ OOP Concepts – Encapsulation, class-based design, and modularization.
<br>
🎮 Game Features

🔁 Draw cards from stock to wastepile
🔄 Move cards between tableau columns using valid Solitaire rules
🂱 Build foundations from Ace to King by suit
♻️ Undo moves using a custom stack-based command system
🎨 Unicode suit symbols and color-coded display
🕹️ Command-based gameplay through console
<br>
🛠️ Technologies Used

Language: C++
Console Encoding: wcout, ANSI escape codes for colored text
No STL Used – All data structures manually implemented
<br>
🧱 Main Components

Class	Purpose
Card	Represents a single card with rank, suit, and visibility
List<T>	Custom doubly linked list with iterator support
Stack<T>	Built on top of List<T> for LIFO operations
Command	Stores each move to support undoing
Game	Core logic for deck initialization, shuffling, rendering, and game flow
<br>
▶️ How to Play

Compile the code in Visual Studio or any C++ IDE with Unicode support.
Run the program in the console.
Use the following commands to interact:
