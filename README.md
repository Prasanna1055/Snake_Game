# Snake Game

This project is an implementation of the classic Snake game using JavaScript, leveraging HTML5 canvas for rendering and Object-Oriented Programming (OOP) principles to structure the game's logic. The game features basic gameplay mechanics, including snake movement, collision detection, and scoring. Below is an overview of the project's key components and functionality:

1. Game Mechanics: The snake is controlled using arrow keys and    moves in a grid-based environment. The game features a food object represented by an image that the snake must chase to grow in size.

2. Data Structures: The snake's body is managed as an array of coordinates, which updates as the snake moves. The game's state, including the position of the food and the snake, is tracked using arrays for efficient collision detection and state management.

3. Scoring System: A score counter is displayed at the top-left corner of the game screen. The score increments each time the snake's head coordinates match the food's coordinates, indicating that the snake has successfully consumed the food.

Object Oriented Design:

i. Snake Class: It creates the snake ,updates its position and growth.

ii. Food: Represents the food object and handles its position and rendering.


KEY FEATURES:
  1. Initialization (init Function):

      i)Canvas Setup: Creates and configures a 1000x1000 canvas for drawing.

      ii)Game Context: Obtains the 2D drawing context for rendering.
      iii)Images: Loads images for the food and trophy.

iv)Snake Object: Initializes the snake with its length, color, and movement direction. Defines methods for creating, drawing, and updating the snake.

v)Event Listener: Adds a keypress event listener to handle direction changes based on arrow key inputs.

2. Drawing (draw Function):

i)Clear Canvas: Clears the previous frame.

ii)Draw Snake: Uses the snake’s drawSnake method to render the snake on the canvas.

iii)Draw Food: Renders the food image at its current position.

iv)Draw Score: Displays the score and trophy image on the canvas.

3. Updating (update Function):

i)Update Snake: Uses the snake’s updateSnake method to move the snake, handle food consumption, and check for boundary collisions.

4. Random Food Position (getRandomFood Function):

i)Generate Coordinates: Computes and returns a new random position for the food within the canvas bounds.

5. Game Loop (gameloop Function):

i)Check Game Over: Ends the game if the snake collides with the canvas boundary.

ii)Draw and Update: Calls draw() and update() functions to refresh the game state and render the new frame.

6. Main Execution:

i)Initialization Call: init() initializes the game setup.

ii)Game Loop Interval: Sets up a repeating interval (setInterval) to run the gameloop function every 100 milliseconds, driving the game’s continuous rendering and updating process.
