<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  
</head>
<body style="font-family: 'Segoe UI', sans-serif; background-color: #121212; color: #f0f0f0; padding: 40px; line-height: 1.6;">

  <h1 style="font-size: 38px; color: #00d4ff;">♠️ Solitaire Game – Data Structures Project (C++)</h1>

  <h2 style="font-size: 28px; color: #ffa500;">📘 Project Overview</h2>
  <p style="font-size: 16px;">
    This is a console-based Solitaire game implemented in C++ as part of a Data Structures assignment. The focus is on custom data structure implementation, object-oriented design, and simulation of Solitaire mechanics. STL was deliberately avoided to solidify the understanding of core structures.
  </p>

  <h2 style="font-size: 28px; color: #ffa500;">🧠 What I Learned</h2>
  <ul style="font-size: 16px;">
    <li>✅ Custom <strong>Doubly Linked Lists</strong> for columns and deck</li>
    <li>✅ <strong>Stack</strong> for stockpile, wastepile, and foundations</li>
    <li>✅ Use of <strong>Custom Iterators</strong> for traversals</li>
    <li>✅ <strong>Undo system</strong> using a stack of command objects</li>
    <li>✅ <strong>OOP concepts:</strong> Encapsulation, inheritance, modular class design</li>
  </ul>

  <h2 style="font-size: 28px; color: #ffa500;">🎮 Game Features</h2>
  <ul style="font-size: 16px;">
    <li>🔁 Draw cards from stockpile to wastepile</li>
    <li>🔄 Move cards between columns using valid Solitaire rules</li>
    <li>🂱 Build foundations from Ace to King by suit</li>
    <li>♻️ Undo moves with a stack-based command system</li>
    <li>🎨 Unicode suits and ANSI color-coded output for visual clarity</li>
    <li>🕹️ Command-based text input interface (no GUI)</li>
    <li>🏆 Win condition check when all 4 foundations reach a King</li>
  </ul>

  <h2 style="font-size: 28px; color: #ffa500;">🛠️ Technologies Used</h2>
  <ul style="font-size: 16px;">
    <li><strong>Language:</strong> C++</li>
    <li><strong>Environment:</strong> Windows Console (Visual Studio)</li>
    <li><strong>Encoding:</strong> Unicode output with <code>wcout</code> & ANSI escape codes</li>
    <li><strong>No STL Used:</strong> All structures (List, Stack, Iterator) were manually implemented</li>
  </ul>

  <h2 style="font-size: 28px; color: #ffa500;">🧱 Main Components</h2>
  <table style="width: 100%; font-size: 16px; border-collapse: collapse;">
    <tr style="background-color: #1e1e1e;">
      <th style="text-align: left; padding: 10px;">Class</th>
      <th style="text-align: left; padding: 10px;">Purpose</th>
    </tr>
    <tr>
      <td style="padding: 10px;">Card</td>
      <td style="padding: 10px;">Represents a card with suit, rank, and visibility state</td>
    </tr>
    <tr>
      <td style="padding: 10px;">List</td>
      <td style="padding: 10px;">Custom doubly linked list with iterator support</td>
    </tr>
    <tr>
      <td style="padding: 10px;">Stack</td>
      <td style="padding: 10px;">Built on top of List for stockpile, wastepile, and foundation piles</td>
    </tr>
    <tr>
      <td style="padding: 10px;">Command</td>
      <td style="padding: 10px;">Stores player moves to support the undo feature</td>
    </tr>
    <tr>
      <td style="padding: 10px;">Game</td>
      <td style="padding: 10px;">Manages deck creation, shuffling, move validation, and game logic</td>
    </tr>
  </table>

  <h2 style="font-size: 28px; color: #ffa500;">▶️ How to Play</h2>
  <p style="font-size: 16px;">
    Compile using Visual Studio or any IDE that supports Unicode console output. Run the program and interact using typed commands:
  </p>

  <h3 style="font-size: 22px; color: #ff69b4;">🔧 Commands</h3>
  <ul style="font-size: 16px;">
    <li><code>s</code> – Draw a card from the stockpile</li>
    <li><code>m c1 c2 n</code> – Move n cards from Column 1 to Column 2</li>
    <li><code>m c1 f1 1</code> – Move top card from Column 1 to Foundation 1</li>
    <li><code>m w c1 1</code> – Move top card from Waste to Column 1</li>
    <li><code>m f1 c1 1</code> – Move card from Foundation 1 to Column 1</li>
    <li><code>z</code> – Undo last command</li>
  </ul>

  <h2 style="font-size: 28px; color: #ffa500;">🏁 Win Condition</h2>
  <p style="font-size: 16px;">
    The game is won when all four foundation stacks contain 13 cards each, ending with the King of each suit.
  </p>

</body>
</html>

