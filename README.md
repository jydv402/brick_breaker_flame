# **Brick Breaker Game** 🧱

This is a brick breaker game built with Flutter and the Flame game engine. It's an example project from a learning path for Flame, designed to teach game development fundamentals on the Flutter framework.

## **Features** 🎮

* **Classic Gameplay**: The game includes all the classic elements: a ball, a player-controlled bat, and bricks to break.
* **Collision Detection**: It uses Flame's `HasCollisionDetection` mixin to handle collisions between game components like the ball, bat, and bricks.
* **Scoring System**: The game tracks the player's score, which is updated whenever a brick is destroyed.
* **Game States**: The game manages different states, including `welcome`, `playing`, `gameOver`, and `won`, each with a corresponding overlay screen.
* **Mobile and Desktop Controls**: Players can control the bat using either arrow keys on a keyboard or by dragging on the screen. The game also supports tapping or pressing the space/enter key to start the game.
* **Responsive Design**: The game camera is set with a fixed resolution, and the components are sized relative to the game's width and height, ensuring a consistent layout across different screen sizes.

***

## **Project Structure** 📁

The project has a clear directory structure for organizing its components:

* `lib/main.dart`: The entry point of the application.
* `lib/src/`: Contains the core game logic.
* `lib/src/brick_breaker.dart`: Defines the main `BrickBreaker` game class, handling game states and logic.
* `lib/src/config.dart`: Stores all the constants for the game's environment, components, and colors.
* `lib/src/components/`: Holds the game objects as individual components.
    * `ball.dart`: Defines the `Ball` component and its collision behavior.
    * `bat.dart`: Defines the `Bat` component with drag and keyboard controls.
    * `brick.dart`: Defines the `Brick` component and what happens when it's hit.
    * `play_area.dart`: Defines the game's play area boundary.
* `lib/src/widgets/`: Contains the Flutter widgets used in the UI layer.
    * `game_app.dart`: The root widget for the application, which sets up the `GameWidget` and overlays.
    * `overlay_screen.dart`: A reusable widget for displaying welcome, game over, and win screens.
    * `score_card.dart`: A widget to display the current score.

***
## (**Steps followed**)[steps.md]
