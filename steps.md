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


    id1 --> id2
    id2 --> id3
    id3 --> id4
    id4 --> id5

```


# Notes
- Where Flutter has `Widgets`, Flame has `Components`. Where Flutter apps consist of creating trees of widgets, Flame games consist of maintaining trees of components.