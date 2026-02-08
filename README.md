# 🧬 Conway's Game of Life Simulation

This project is a Python implementation of **Conway's Game of Life**, a cellular automaton zero-player game. It demonstrates algorithmic logic, matrix manipulation, and data visualization using **Matplotlib**.

## 🎮 How It Works
The universe of the Game of Life is an infinite, two-dimensional orthogonal grid of square cells, each of which is in one of two possible states: **alive** or **dead**. Every cell interacts with its eight neighbours, which are the cells that are horizontally, vertically, or diagonally adjacent.

### The Rules
At each step in time, the following transitions occur:
1.  **Underpopulation**: Any live cell with fewer than two live neighbours dies.
2.  **Survival**: Any live cell with two or three live neighbours lives on to the next generation.
3.  **Overpopulation**: Any live cell with more than three live neighbours dies.
4.  **Reproduction**: Any dead cell with exactly three live neighbours becomes a live cell.

## 🚀 Features
* **Object-Oriented Design**: Encapsulated logic within a `GameOfLife` class.
* **Custom Population**: Users can initialize the grid with specific coordinate patterns (e.g., Gliders, Blinkers).
* **Visualization**: Uses `matplotlib.pyplot` to render the grid state visually.
* **Simulation**: Supports stepping through generations one by one or in batches.

## 🛠️ Tech Stack
* **Python 3.8+**
* **Matplotlib** (Visualization)
* **IPython** (Dynamic output handling)

## 🏃‍♂️ Usage

1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/conways-game-of-life.git](https://github.com/YOUR_USERNAME/conways-game-of-life.git)
    ```

2.  **Run the Notebook**:
    Open `game_of_life.ipynb` in Jupyter Notebook or VS Code and run the cells to watch the simulation evolve.

3.  **Example Code**:
    ```python
    game = GameOfLife(10, 10)
    game.populate_grid([(1, 2), (2, 3), (3, 1), (3, 2), (3, 3)]) # Glider Pattern
    game.make_n_steps(5)
    game.draw_grid()
    ```

## 📜 Credits
Completed as part of the **365 Data Science** Python Bootcamp.
