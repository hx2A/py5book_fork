# is_looping

Boolean value reflecting if the Sketch is looping.

## Examples

<div class="example-table">

<div class="example-row"><div class="example-cell-image">

</div><div class="example-cell-code">

```python
x = 0.0


def setup():
    py5.size(200, 200)


def draw():
    global x
    py5.background(204)
    py5.line(x, 0, x, py5.height)
    x = x + 1
    if x > py5.width:
        x = 0


def mouse_pressed():
    if py5.is_looping:
        py5.no_loop()
    else:
        py5.loop()
```

</div></div>

</div>

## Description

Boolean value reflecting if the Sketch is looping. This will be `True` by default, and `False` after [](sketch_no_loop) has been called. Calling [](sketch_loop) will set it back to `True`.

Underlying Processing field: isLooping

Updated on October 26, 2026 15:22:53pm UTC
