# A-Mazing Game
[Live Site!](https://arittrosaha.github.io/A-Mazing-Game/)

Note - The application is hosted in GitHub.

## Summary
**Synopsis** - It is a maze game and a graph algorithm simulator that uses algorithms and data structures to generate and solve mazes while also giving an option for a player to solve the maze by themselves. It is coded with vanilla JS and rendered using HTML5 Canvas.

**Stack** - JS, HTML5, CSS3, Canvas.

**Key Points**:
* Implemented graph traversal algorithms such as DFS and BFS to generate and solve mazes.
* Built a customized algorithm to calculate the 2D position of a node in a 1D array.
* Performed dynamic DOM manipulation with just vanilla JavaScript.


## How does it work?

<img src="gifs/solve_maze.gif" alt="Solve Maze" align = "right" />
<img src="gifs/generate_maze.gif" alt="Generate Maze" align = "right" />

Step 1 (Generate Maze) - Select difficulty level between Easy, Medium and Hard to generate an easy, medium or hard maze respectively. All levels of maze generation is done using a DFS algorithm, currently.

Step 2 (Solve Maze) - Select a mode to solve the maze from the following options:
* DFS - The maze will be solved using a DFS algorithm.
* BFS - The maze will be solved using a BFS algorithm.
* Solve Yourself - Use the up, down, left and right arrow keys to navigate through the maze. But if you hit a wall, you will start over.



## Detailed Breakdown
### Keys
<img src="images/keys.png" alt="Keys" />

* **White** indicates walls.
* **Red** indicates maze path.
* **Light Blue** indicates the target or finish.
* **Gree** indicates portion of the maze that has been explored.
* **Dark Blue** indicates the shortest path from finish to back start.

### Setup
| Grid | Cell |
-------|-------


### Generate Maze
| Render | Code Snippet |
---------|---------------
<img src="gifs/hard_generate.gif" alt="Generating a hard maze" />|<img src="images/dfs_gen.png" alt="Code snippet for generateing a maze with DFS" />

**Render** - This is a visulization of a generating maze with DFS after the Hard button is pressed.

**Code Snippet** - This is a portion of the code to render and create a maze using HTML5 and DFS algorithm, respectively. This is an itterative implementation of DFS. 
* Animation rate - The need for a continuous loop and a way to control the rate of animation is achieved by the use of setInterval asynchronous function. While 0 milliseconds is passed in this setInterval function (code not visible in this snippet), the minimum default time value is 4ms for HTML5. Therefore, the frame rate is 1 frame per 4 ms.
* Line 41 to 55 - The main portion of the code handling the DFS logic.
* Line 57 and bellow - Selects a random target from the last row.

### Solve Maze



## Future Plans
### Generating the maze
A player will need to make two choice to generate a map:
* A Difficulty level from Easy, Medium or Hard
* An Algorithm from DFS, BFS, Kruskal's, Prim's or Obstacle based test cases for A*

### Solving the maze
**Algorithms**:
  * Upcoming ones - Dijkstra's, A*, Prim's or Kruskal's
  * Last time, average time and number of times run for the current player to solve the current map will be displayed per algorithm.

**Solving Yourself**:
  * Top 10 lowest time will be displayed alongside a provided username, that is appropriate, per level bellow the map.
  * A countdown will be displayed as soon as a human clicks the Solving Yourself button and will run until the target is reached.
    
