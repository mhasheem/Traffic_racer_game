
# Traffic Racer Game

**Traffic Racer** is a simple CLI-based car racing game written in C. The game allows players to navigate a car through different lanes while avoiding obstacles. It demonstrates fundamental game development concepts such as handling user input, rendering graphics to the console, and managing game state.


## Game Overview

Traffic Racer is a console application designed to run in a Windows environment. The game features a car that moves horizontally across lanes, and the objective is to avoid obstacles that appear randomly. Players use arrow keys to maneuver the car and try to achieve the highest score possible.

## Major Components

- **`main()`**: The entry point of the game, which initializes the game state and handles the main game loop.
- **`newpos(int in, int *px)`**: Updates the car's position based on user input.
- **`printcar(int *px, int *py)`**: Renders the car on the console screen.
- **`printroad()`**: Draws the road and lane markings on the console.
- **`obstacles()`**: Manages the generation and movement of obstacles.
- **`collision(int *px, int *py)`**: Detects collisions between the car and obstacles.

## Code Explanation

### `main()`

- **Purpose**: Initializes game parameters and enters the main game loop.
- **Key Actions**:
  - Displays game instructions and waits for the player to press 'S' to start.
  - Contains the main game loop, which updates the car's position, prints the road, car, and obstacles, and checks for collisions.

### `newpos(int in, int *px)`

- **Purpose**: Adjusts the car’s horizontal position based on user input.
- **Key Actions**:
  - Moves the car left or right by updating its position based on the arrow keys pressed.

### `printcar(int *px, int *py)`

- **Purpose**: Renders the car at its current position on the screen.
- **Key Actions**:
  - Constructs a string representation of the car based on its position and prints it to the console.

### `printroad()`

- **Purpose**: Draws the road and lane markings.
- **Key Actions**:
  - Prints multiple lines to represent the lanes and road width, creating a visual guide for the gameplay.

### `obstacles()`

- **Purpose**: Generates and moves obstacles on the road.
- **Key Actions**:
  - Randomly places obstacles in different lanes and manages their movement down the screen.

### `collision(int *px, int *py)`

- **Purpose**: Checks for collisions between the car and obstacles.
- **Key Actions**:
  - Detects if the car's current lane intersects with an obstacle's position.
  - Updates the score and displays a collision message if an obstacle is hit.


## Controls

- **Arrow Keys**: Move the car left and right.
- **'S' Key**: Start the game.

## Gameplay

- **Objective**: Navigate the car through lanes and avoid obstacles.
- **Scoring**: Points are awarded based on how long you survive and avoid obstacles. The game keeps track of the highest score.

## Known Issues

- **Obstacle Overlap**: There may be occasional overlaps or gaps in obstacle placement.
- **Screen Flickering**: Frequent clearing of the screen may cause flickering on some systems.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
