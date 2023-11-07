# GDScript

*- programming language for Godot.*

## Initialization

```gd
## Nodes are initialized by top-down approach.
## +-----------------------------------------------+
## |NODE           _init()  _enter_tree()  _ready()|
## |-----------------------------------------------|
## |parent         (01)     (08)           (21)    |
## |  child_1       (02)     (09)           (17)   |
## |    child_1_a    (03)     (10)           (15)  |
## |    child_1_b    (04)     (11)           (16)  |
## |  child_2       (05)     (12)           (20)   |
## |    child_2_a    (06)     (13)           (18)  |
## |    child_2_b    (07)     (14)           (19)  |
## +-----------------------------------------------+

## Called on start.
func _init():
    pass

## Called on start after all nodes in tree are "initialized".
func _enter_tree():
    pass

## Called on start after all nodes in tree "entered tree" and also all child
## nodes are "ready".
func _ready():
    pass
```

## Continuation

```gd
## Called every frame (FPS/s).
## - delta = time in seconds between refreshes.
func _process(delta):
    pass

## Called at fixed rate (60/s by default).
## - delta = time in seconds between refreshes.
func _physics_process(delta):
    pass
```

## Input

```gd
```
