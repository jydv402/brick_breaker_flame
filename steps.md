```mermaid
---
title: Flame tutorial steps (Creating a brick breaker game)
---
flowchart TD
    id1(Create the main.dart file)
    id2(Create the config.dart file insided lib/src)
    id3(Create the PlayArea component)
    id4(Create components.dart file)
    id5(Create the brick_breaker.dart file)
    id6(Create the ball component)
    id7(Add the ball component to the world and give random motion for now)
    id8(Trying to add collision detection for the ball)
    id9(Create a BAT component)
    id10(Add the BAT component to the WORLD)
    id11(Create the Brick components)
    id12(Add the bricks to the world)
    id13(Created the game, now all left is to polish it)


    id1 --> id2 --> id3 --> id4 --> id5 --> id6 --> id7 --> id8 --> id9 --> id10 --> id11 --> id12 --> id13

```


# Notes
- Where Flutter has `Widgets`, Flame has `Components`. Where Flutter apps consist of creating trees of widgets, Flame games consist of maintaining trees of components.
- The background/PlayArea is a `RectangleComponent` and the Ball is a `CircleComponent`
- For collision -> First, the code tests if the `Ball` collided with `PlayArea`. This seems redundant for now, as there are no other components in the game world. That will change in the next step, when you add a bat to the world. Then, it also adds an else condition to handle when the ball collides with things that aren't the bat. A gentle reminder to implement remaining logic, if you will.
- Cuurently a fixed number of bricks are produced
- Every component has a `CollisionCallbacks` for collisions and `HasGameReference<BrickBreaker>` for referencing to the PlayArea