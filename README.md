# Chess Game using Minimax Algorithm

## 📌 Introduction
This project is a **Chess Game** built using JavaScript, featuring an AI opponent powered by the **Minimax Algorithm**. The game allows human vs AI and human vs human modes, with AI making optimal moves based on the minimax strategy.

## ℹ️ About the Project
The **Chess Game** implements the Minimax algorithm with Alpha-Beta pruning to optimize AI decision-making. The game provides a smooth user experience with an interactive UI, drag-and-drop functionality, and move validation. The AI evaluates board positions and selects the best possible moves to challenge players effectively.

## 🚀 Features
✔ **Play against AI or another player**  
✔ **Minimax Algorithm with Alpha-Beta Pruning**  
✔ **Drag and drop pieces for easy gameplay**  
✔ **Move validation and checkmate detection**  
✔ **Responsive design for all screen sizes**  
✔ **Undo move functionality**

## 📂 Folder Structure
```
Chess/
│── Board.js          # Manages the chessboard state
│── Game.js           # Handles game flow and logic
│── History.js        # Tracks move history
│── SimulationGame.js # Simulates moves for AI evaluation
│── ai.js             # Implements Minimax AI with Alpha-Beta Pruning
│── piece.js          # Defines chess piece movement and rules
│── chess.html        # Main HTML file for UI
│── chess.css         # Styling for the chessboard
│── favicon.ico       # Icon for the game
│── LICENSE           # License file
│── README.md         # Documentation
```
```
Chess/
│── src/             # JavaScript source code
│── assets/          # Images and sounds
│── index.html       # Main game file
│── style.css        # Styling for the board
│── script.js        # Game logic and AI
│── README.md        # Documentation
│── LICENSE          # License file
```

## 🔧 Installation & Usage
1. **Clone the repository:**
   ```bash
   git clone https://github.com/subhm2004/Chess.git
   ```
2. **Navigate to the directory:**
   ```bash
   cd Chess
   ```
3. **Open `index.html` in a browser** to start playing.

## 🎮 How the AI Works
The AI in this chess game is powered by the **Minimax Algorithm**, a decision-making algorithm used for turn-based strategy games. The core idea of Minimax is to evaluate all possible future game states and choose the move that minimizes the opponent's advantage while maximizing the AI's winning chances.

### 🔍 Minimax Algorithm Explained
1. **Game Tree Construction**: The AI generates a tree of all possible moves up to a certain depth, analyzing the outcomes of each move.
2. **Min and Max Levels**: The tree alternates between maximizing (AI's turn) and minimizing (opponent's turn) scores, ensuring the AI picks the best possible move.
3. **Evaluation Function**: Each board position is scored using a heuristic function that considers factors like piece value, mobility, control of the board, and checkmate threats.
4. **Recursive Exploration**: The algorithm recursively explores future moves, simulating multiple turns ahead, and assigns scores based on possible outcomes.
5. **Optimal Move Selection**: After analyzing all possible moves, the AI selects the move that leads to the most favorable board state while assuming the opponent plays optimally.

### ⚡ Alpha-Beta Pruning Optimization
Minimax can be computationally expensive, so **Alpha-Beta Pruning** is implemented to reduce the number of nodes evaluated in the search tree. It works by:
- **Pruning unnecessary branches**: If a move is already proven to be worse than a previously examined move, further exploration of that branch is skipped.
- **Reducing search time**: This significantly improves efficiency, allowing deeper move analysis in the same amount of time.

### 📊 Evaluation Function Details
The evaluation function is crucial for AI performance and considers:
- **Material Advantage**: Assigns points to pieces (Pawn = 1, Knight/Bishop = 3, Rook = 5, Queen = 9).
- **Piece Mobility**: Encourages moves that increase the number of available legal moves.
- **King Safety**: Ensures that the AI prioritizes moves that protect its king.
- **Center Control**: Encourages controlling the central squares (d4, d5, e4, e5) for strategic dominance.

### ♟️ Why Minimax for Chess?
✔ Ensures AI makes **strategically sound** moves.  
✔ Simulates **multiple turns ahead** for better decision-making.  
✔ Works well with **heuristic evaluation functions**.  
✔ Efficient with **Alpha-Beta Pruning**, allowing deeper analysis.  

This combination of **Minimax + Alpha-Beta Pruning** results in a challenging AI opponent that can compete effectively against human players.
The AI in this chess game is powered by the **Minimax Algorithm**, a decision-making algorithm used for turn-based strategy games. The core idea of Minimax is to evaluate all possible future game states and choose the move that minimizes the opponent's advantage while maximizing the AI's winning chances.

### 🔍 Minimax Algorithm Explained
1. **Game Tree Construction**: The AI generates a tree of all possible moves up to a certain depth.
2. **Min and Max Levels**: The tree alternates between maximizing (AI's turn) and minimizing (opponent's turn) scores.
3. **Evaluation Function**: Each board position is scored using a heuristic function that considers factors like piece value, board control, and threats.
4. **Recursive Exploration**: The algorithm recursively explores future moves and assigns scores based on possible outcomes.
5. **Optimal Move Selection**: The AI selects the move that leads to the highest score while assuming the opponent plays optimally.

### ⚡ Alpha-Beta Pruning Optimization
To improve efficiency, Alpha-Beta Pruning is used to eliminate branches of the tree that don’t need to be explored, significantly reducing computation time.

### ♟️ Why Minimax for Chess?
✔ Ensures AI makes optimal moves 
✔ Simulates multiple turns ahead 
✔ Works well with heuristic evaluation 
✔ Efficient with Alpha-Beta Pruning
The AI uses the **Minimax Algorithm** to evaluate the best possible move by simulating future positions and choosing the most optimal one. Alpha-Beta Pruning is implemented to reduce computation time by eliminating unnecessary calculations.

## 🤝 Contributing
Contributions are welcome! Feel free to create a pull request for improvements or bug fixes.

## 📜 License
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---
🔗 **GitHub Repo:** [Chess Game](https://github.com/subhm2004/Chess.git)  
👨‍💻 **Author:** Shubham Malik  
📧 **Email:** subhu04012003@gmail.com

