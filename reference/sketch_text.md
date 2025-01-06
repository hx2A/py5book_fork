# text()

Draws text to the screen.

## Examples

<div class="example-table">

<div class="example-row"><div class="example-cell-image">

![example picture for text()](/images/reference/Sketch_text_0.png)

</div><div class="example-cell-code">

```python
def setup():
    py5.text_size(32)
    py5.text("word", 10, 30)
    py5.fill(0, 102, 153)
    py5.text("word", 10, 60)
    py5.fill(0, 102, 153, 51)
    py5.text("word", 10, 90)
```

</div></div>

<div class="example-row"><div class="example-cell-image">

![example picture for text()](/images/reference/Sketch_text_1.png)

</div><div class="example-cell-code">

```python
def setup():
    py5.size(100, 100, py5.P3D)
    py5.text_size(32)
    py5.fill(0, 102, 153, 204)
    py5.text("word", 12, 45, -30)  # specify a z-axis value
    py5.text("word", 12, 60)  # default depth, no z-value specified
```

</div></div>

<div class="example-row"><div class="example-cell-image">

![example picture for text()](/images/reference/Sketch_text_2.png)

</div><div class="example-cell-code">

```python
def setup():
    s = "The quick brown fox jumps over the lazy dog."
    py5.fill(50)
    py5.text(s, 10, 10, 70, 80)  # text wraps within text box
```

</div></div>

</div>

## Description

Draws text to the screen. Displays the information specified in the first parameter on the screen in the position specified by the additional parameters. A default font will be used unless a font is set with the [](sketch_text_font) function and a default size will be used unless a font is set with [](sketch_text_size). Change the color of the text with the [](sketch_fill) function. The text displays in relation to the [](sketch_text_align) function, which gives the option to draw to the left, right, and center of the coordinates.

The `x2` and `y2` parameters define a rectangular area to display within and may only be used with string data. When these parameters are specified, they are interpreted based on the current [](sketch_rect_mode) setting. Text that does not fit completely within the rectangle specified will not be drawn to the screen.

Note that py5 lets you call `text()` without first specifying a Py5Font with [](sketch_text_font). In that case, a generic sans-serif font will be used instead. (See the third example.)

Underlying Processing method: [text](https://processing.org/reference/text_.html)

## Signatures

```python
text(
    c: chr,  # the alphanumeric character to be displayed
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    /,
) -> None

text(
    c: chr,  # the alphanumeric character to be displayed
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    z: float,  # z-coordinate of text
    /,
) -> None

text(
    chars: Iterator[chr],  # the alphanumberic symbols to be displayed
    start: int,  # array index at which to start writing characters
    stop: int,  # array index at which to stop writing characters
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    /,
) -> None

text(
    chars: Iterator[chr],  # the alphanumberic symbols to be displayed
    start: int,  # array index at which to start writing characters
    stop: int,  # array index at which to stop writing characters
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    z: float,  # z-coordinate of text
    /,
) -> None

text(
    num: float,  # the numeric value to be displayed
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    /,
) -> None

text(
    num: float,  # the numeric value to be displayed
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    z: float,  # z-coordinate of text
    /,
) -> None

text(
    num: int,  # the numeric value to be displayed
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    /,
) -> None

text(
    num: int,  # the numeric value to be displayed
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    z: float,  # z-coordinate of text
    /,
) -> None

text(
    str: str,  # string to be displayed
    x1: float,  # by default, the x-coordinate of text, see rectMode() for more info
    y1: float,  # by default, the y-coordinate of text, see rectMode() for more info
    x2: float,  # by default, the width of the text box, see rectMode() for more info
    y2: float,  # by default, the height of the text box, see rectMode() for more info
    /,
) -> None

text(
    str: str,  # string to be displayed
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    /,
) -> None

text(
    str: str,  # string to be displayed
    x: float,  # x-coordinate of text
    y: float,  # y-coordinate of text
    z: float,  # z-coordinate of text
    /,
) -> None
```

Updated on January 06, 2025 23:06:20pm UTC
