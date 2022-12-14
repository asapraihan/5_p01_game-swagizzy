# Project 01 For NeXT CS
### Class Period: 5
### Name0: Izzy
---


Your mission is to recreate one of these two classic arcade games:
- Breakout/Arkanoid [demo 0](https://elgoog.im/breakout/)  [demo 1](https://www.crazygames.com/game/atari-breakout)
- Space Invaders [demo 0](https://elgoog.im/space-invaders/) [demo 1](https://www.crazygames.com/game/space-invaders)

This project will be completed in phases. The first phase will be to work on this document. Use makrdown formatting. For more markdown help [click here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) or [here](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)


---

## Phase 0: Game Selection, Analysis & Plan

#### Selected Game: Breakout/Arkanoid

### Necessary Features
What are the core features that your game should have? These should be things that __must__ be implemented in order to make the game playable, not extra features that could be added to make the game more fun to play.

-paddle that can be moved horizontally with mouse, bounces ball back 
-ball that starts in the middle, breaks bricks that it touches, bounces back to the opposite direction it hits after touching brick or the walls
-bricks that are part of the arrays that get broken 
-direction of where ball bounces depends on where on the paddle it hits


### Extra Features
What are some features that are not essential to gameplay, but you would like to see (provided you have time after completing the necessary features.

-number that says how many bricks are left
-pause feature 
-game resets when the player has no more lives
-3 lives, ball and paddle starts at middle but bricks aren't reset, game resets when it hits 0 lives


### Controls
How will your game be controlled? If the mouse will be used, explain how. List all keyboard commands as well.

Keyboard Commands:
- spacebar to pause/continue the game

Mouse Conrol:
- Mouse movement: left/right to move paddle
- Mouse pressed: start the game


### Classes
What classes will you be creating for this project? Include the instance variables and methods that you believe you will need. You will be required to create at least 2 different classes. If you are going to use classes similar to those we've made for previous assingments, you will have to add new features to them.


CLASS paddle
- Instance variables:
  - x
  - y
  - width
  - height
- METHODS
  - move()
  - display()
  - ballHit()
  - reset()

CLASS ball
- Instance variables:
  - x
  - y
  - xVelocity
  - yVelocity
  - radius
- METHODS
  - display()
  - move()
  - xMove(direction)
  - yMove(direction)
  - reset()
  
  CLASS brick
- Instance variables:
  - x
  - y
  - width
  - height
  - state
- METHODS
  - display()
  - break()
  - hitLeft()
  - hitRight()
  - hitTop()
  - hitBottom()
  - reset()

 CLASS brickGrid
- Instance variables:
  - numRows
  - numCols
  - grid
- METHODS
  - setupGrid()
  - showGrid()
  - updateGrid()
  - scoreCalc()
