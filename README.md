# Maze Pathfinding Visualizer 🧭

A terminal-based maze solver using **Breadth-First Search (BFS)** and `curses` for live visualization.

## 🚀 Features

- Visual pathfinding from start (`O`) to end (`X`)
- Real-time animation of the search algorithm
- Maze visualized directly in your terminal with colors

## 📦 Requirements

- Python 3.x
- `curses` module (comes built-in with Unix; for Windows, use [windows-curses](https://pypi.org/project/windows-curses/))

## 🧠 How it Works

- The maze is a 2D grid of characters:
  - `#` = Wall  
  - `' '` = Open path  
  - `O` = Start  
  - `X` = End  
- BFS is used to find the shortest path from start to finish.
- As BFS explores, the terminal updates live to show visited paths in **red** and unvisited in **blue**.

## ▶️ How to Run

### On Linux/macOS:

```bash
python3 maze_solver.py
```

### On Windows:

```bash
pip install windows-curses
python maze_solver.py
```

## 🛠 Customizing the Maze

Modify the `maze` variable directly in the code. Example:

```python
maze = [
    ["#", "O", "#"],
    ["#", " ", "#"],
    ["#", "X", "#"]
]
```

Make sure:
- There’s one `O` (start) and one `X` (end)
- At least one valid path exists between them



**Live pathfinding in red as it finds the way!**

---

## 📚 License

MIT License. Free to use, modify, and distribute.
