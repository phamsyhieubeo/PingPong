<h1>IST ASSESSMENT</h1>
<h2>Sy Hieu Pham</h2>

```markdown
# Ping Pong Game

## Overview

This is a simple Ping Pong game made with Python. You can control paddles and hit the ball, just like in the old Pong games. You can also change settings, and the game has a menu to help you start or learn how to play.

## Features

- **Main Menu**: Start the game, go to settings, or see how to play.
- **Paddle Controls**: 
  - Player A: Use `W` to move up and `S` to move down.
  - Player B: Use the `Up Arrow` to move up and the `Down Arrow` to move down.
- **Settings**: You can change the shape of the ball (either a square or a circle).
- **Other Controls**:
  - Press `R` to reset the game.
  - Press `ESC` to quit the game.

## How to Play

1. Open the main menu and click "Start" to begin the game.
2. Player A uses the `W` and `S` keys to move the paddle.
3. Player B uses the `Up Arrow` and `Down Arrow` keys to move the paddle.
4. The ball will bounce off the top and bottom walls. If it goes past a paddle, the other player gets a point.
5. The scores are shown at the top of the screen.

## Installation

1. Download or clone this project:
   `git clone <repository-url>`
  
2. Make sure you have Python installed on your computer.
3. Run the game with:
   `python <filename>.py`

## Game Controls

- **W/Up Arrow**: Move the paddle up.
- **S/Down Arrow**: Move the paddle down.
- **R**: Reset the game score.
- **ESC**: Exit the game.

## Settings

You can change the shape of the ball in the **Settings** menu. The options are:
- **Square**
- **Circle**

The settings are saved in a file called `Setting.json`, so they will stay the same next time you play.

## How to Change the Game

- You can change the speed of the ball or other things in the game by editing the code.
- The main menu and settings can also be changed easily by modifying the `main_menu()` function in the code.
- You can also change the settings in the `Setting/Setting.json` file to directly adjust the ball shape or other options.
 ```



```markdown
# Ping Pong Game

## Functions Explained

### `main_menu()`

The `main_menu()` function is the first screen that appears when you start the game. It creates a window with the title "PING PONG" and several buttons. These buttons allow you to start the game, go to the settings, see how to play, or quit the game. 

In this function:
- The `Start` button starts the game.
- The `Setting` button opens the settings menu where you can change the ball shape.
- The `How to play` button shows a popup with the game controls.
- The `Quit` button closes the game.

### `HowToPlay()`

The `HowToPlay()` function opens a message box that tells the player how to control the paddles:
- `W` and `S` keys to move the left paddle (Player A).
- `Up Arrow` and `Down Arrow` keys to move the right paddle (Player B).
- `R` to reset the game.
- `ESC` to quit.

### `Setting_func()`

The `Setting_func()` function opens the settings menu. In this menu, you can change the shape of the ball to either a square or a circle. When you click the "Apply" button, the selected shape is saved in the `Setting.json` file, so it is remembered the next time you play. 

In this function:
- You can choose the ball shape using a dropdown menu.
- You can go back to the main menu by clicking "Back".
- The "Apply" button saves your selected settings.

### `GamePlay()`

The `GamePlay()` function starts the actual Ping Pong game. It creates the window where the game is played. The paddles and ball are drawn on the screen, and the game begins. 

In this function:
- Player A controls the left paddle with the `W` and `S` keys.
- Player B controls the right paddle with the `Up Arrow` and `Down Arrow` keys.
- The ball bounces around, and the players try to stop it from going past their paddles.
- Scores are updated whenever a player misses the ball.
- The `R` key resets the game, and the `ESC` key quits the game.

### `apply()`

The `apply()` function is inside the `Setting_func()` and is used to save your chosen ball shape to the `Setting.json` file. After you select either "circle" or "square" from the dropdown menu and click "Apply," this function updates the settings.

### `back()`

The `back()` function is also part of the `Setting_func()`. It simply takes you back to the main menu by hiding the settings screen and showing the main menu again.

### `pad_a_up()` and `pad_a_down()`

These functions control the movement of the left paddle (Player A). 
- `pad_a_up()` moves the left paddle up by 20 units.
- `pad_a_down()` moves the left paddle down by 20 units.

### `pad_b_up()` and `pad_b_down()`

These functions control the movement of the right paddle (Player B).
- `pad_b_up()` moves the right paddle up by 20 units.
- `pad_b_down()` moves the right paddle down by 20 units.

### `ex()`

The `ex()` function allows you to quit the game by closing the game window.

### `reset()`

The `reset()` function resets the game by setting the ball back to the middle of the screen and resetting both players' scores to 0.

---

This explanation covers the main functions in the game and what they do. Each function has a specific purpose, like starting the game, moving paddles, or updating settings.
```
