# Robot Path Simulation
## Overview

his program simulates the movement of a robot on a grid-based map loaded from a file (map.txt). The robot starts at the center of the map and moves in a random direction, avoiding obstacles while consuming fuel. The simulation is run three times to demonstrate different possible paths. Additionally, the robot must carefully manage its fuel and ensure that it returns to the starting point (base) before running out of fuel in order not to lose points.

The robot moves randomly in one direction as long as it has fuel and there are no obstacles. If it can't move in the current direction, it will turn left, and if that doesn't work, it will turn right. If it still can't move, it will turn around and head back to the base.

## Features

Reads a grid-based map from a file.

Randomly selects a movement direction (left, right, up, or down).

Moves in the chosen direction while avoiding obstacles (-1 in the matrix).

Uses a stack to track the robot's path.

Displays the path taken and the number of points collected.

## File Structure

- main.cpp - Contains the implementation of the robot movement simulation.

- map.txt - The map file that defines the grid (must be present in the same directory as the executable).

## Map File Format (map.txt)

### The map.txt file should contain:

The number of rows and columns of the grid.

A matrix where each cell represents a position:

  - -1 for obstacles.

  - any other number for open paths.

### Example map.txt:
![image](https://github.com/user-attachments/assets/72714c24-303c-45f8-9d22-8bf7e51600e9)

## How It Works

The program prompts the user to enter a fuel amount.

It runs the simulation three times, each time choosing a different random direction.

The robot moves within the given fuel constraints while avoiding obstacles.

The robot's path and points collected are displayed.

### Example Output:
![image](https://github.com/user-attachments/assets/7cbe45b0-88ef-400d-8b05-7e3f4bdf0245)

