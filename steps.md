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
    id9(Add a BAT component)


    id1 --> id2
    id2 --> id3
    id3 --> id4
    id4 --> id5
    id5 --> id6
    id6 --> id7
    id7 --> id8 --> id9

```


# Notes
- Where Flutter has `Widgets`, Flame has `Components`. Where Flutter apps consist of creating trees of widgets, Flame games consist of maintaining trees of components.
- The background/PlayArea is a `RectangleComponent` and the Ball is a `CircleComponent