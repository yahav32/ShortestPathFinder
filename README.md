# Shortest Path Finder

A terminal-based interactive maze solver visualization implemented in Python using the `curses` library. This project visualizes pathfinding algorithms finding the shortest path between a starting position (`O`) and an ending position (`X`).

## Features

- **Multiple Algorithms**:
  - **A\* Search**: Explores the maze efficiently using a heuristic function (Manhattan distance).
  - **BFS (Breadth-First Search)**: Guarantees the shortest path in unweighted grids.
- **Terminal Visualization**: Real-time visual feedback of the pathfinding process (explored nodes, current path, start/end points, walls).
- **Responsive Error Handling**: Detects terminal window size and warns the user if it's too small for the maze dimensions.

## Requirements

- Python 3.x
- `curses` module (standard library on Unix/Linux/macOS)
- `windows-curses` (required to run on Windows)

## Installation

1. **Clone the repository**:
   ```bash
   git clone <your-repository-url>
   cd ShortestPathFinder
   ```

2. **Set up a virtual environment (optional but recommended)**:
   ```bash
   python -m venv .venv
   ```

3. **Activate the virtual environment**:
   - **Windows (PowerShell)**:
     ```powershell
     .venv\Scripts\Activate.ps1
     ```
   - **Windows (CMD)**:
     ```cmd
     .venv\Scripts\activate.bat
     ```
   - **macOS/Linux**:
     ```bash
     source .venv/bin/activate
     ```

4. **Install dependencies** (if running on Windows):
   ```bash
   pip install windows-curses
   ```

## Running the Application

Ensure your terminal window is expanded, then run:

```bash
python path_finder.py
```

## How It Works

- The grid is defined in `path_finder.py`. You can modify `maze` or `maze2` variables to design your custom mazes.
- `#` represents walls.
- `O` represents the starting point.
- `X` represents the target exit point.
- The visualization uses color-coded symbols:
  - Green `X` for the calculated final path.
  - Yellow `.` for explored/visited positions.
  - Red for the starting/ending points.
  - Blue for the walls.
