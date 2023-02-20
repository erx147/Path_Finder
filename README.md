# Path Finder

This is a Python program that solves a maze using breadth-first search algorithm. It utilizes the curses library to display the maze and the path on the terminal window.

## Usage
To use this program, simply run the following command:
  python path_finder.py

## Dependencies
This program requires Python 3 and the curses library to run. When using a windows machine, the curses library can be installed using pip with the following command:
  pip install windows-curses

## How it works
The program reads in a 2D array that represents the maze, where '#' represents walls and ' ' represents open spaces. It then finds the starting position 'O' and the ending position 'X'.

The program uses a breadth-first search algorithm to find the shortest path from the starting position to the ending position. At each step, the program checks if the current position is the ending position. If it is, the program returns the path that led to that position.

If the current position is not the ending position, the program finds all of the neighboring positions that are not walls, and adds them to a queue along with the path that led to that position. The program then continues searching until it finds the ending position.

The program uses the curses library to display the maze and the path on the terminal window. The print_maze function prints out the maze, with the current path highlighted in red. The main function sets up the curses environment and calls the find_path function to find the shortest path. The find_path function uses the print_maze function to update the terminal window at each step of the search.
