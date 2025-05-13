# Single-Agent Pacman AI
Implementation of Pacman Agent

**Note:** This project was part of the coursework for CSE 473 at the University of Washington.
The majority of the framework as provided by the instructors. My contributions were in:
- search.py
- searchAgents.py

## Overview
The game environment simulates a Pacman game where Pacman must navigate around maze walls while collecting food and optimizing path efficiency. Uses search techniques including:
- Depth-first Search
- Breadth-first Search
- Uniform Cost Search
- A* Search

### Implemented Problems:
**CornersProblem**
- Visits all four corners of a maze
- Tracks current position and visited corners
- Heuristic estimates how far Pacman is from completing task using Manhattan distances to unvisited corners
- Agent uses A* search to prioritize moving quickly towards unvisited corners with no unnecessary movement.

**FoodSearchProblem**
- Collects all food in maze
- States represent current position and food grid for all remaining foods
- Heuristic calculates maze distance from farthest food from Pacman's position
- Agent uses A* search to find a path that efficiently finds all food and prioritizes longer trips earlier when needed.

**ClosestDotSearchAgent**
- Repeatedly finds nearest piece of food until finished with maze
- Uses BFS to follow the path to closest food, then repeats
