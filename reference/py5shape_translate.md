# Py5Shape.translate()

Specifies an amount to displace the shape.

## Examples

<div class="example-table">

<div class="example-row"><div class="example-cell-image">

</div><div class="example-cell-code">

```python
def setup():
    global s
    s = py5.load_shape("bot.svg")


def draw():
    py5.background(204)
    py5.shape(s)


def mouse_pressed():
    # move the shape 10 pixels right each time the mouse is pressed
    s.translate(10, 0)
```

</div></div>

</div>

## Description

Specifies an amount to displace the shape. The `x` parameter specifies left/right translation, the `y` parameter specifies up/down translation, and the `z` parameter specifies translations toward/away from the screen. Subsequent calls to the method accumulates the effect. For example, calling `translate(50, 0)` and then `translate(20, 0)` is the same as `translate(70, 0)`. This transformation is applied directly to the shape, it's not refreshed each time `draw()` is run. 

Using this method with the `z` parameter requires using the `P3D` parameter in combination with size.

Underlying Processing method: [PShape.translate](https://processing.org/reference/PShape_translate_.html)

## Signatures

```python
translate(
    x: float,  # left/right translation
    y: float,  # up/down translation
    /,
) -> None

translate(
    x: float,  # left/right translation
    y: float,  # up/down translation
    z: float,  # forward/back translation
    /,
) -> None
```

Updated on March 06, 2023 02:49:26am UTC
