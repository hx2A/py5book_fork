# Py5Graphics.text_width()

Calculates and returns the width of any character or text string.

## Description

Calculates and returns the width of any character or text string.

This method is the same as [](sketch_text_width) but linked to a `Py5Graphics` object. To see example code for how it can be used, see [](sketch_text_width).

Underlying Processing method: PGraphics.textWidth

## Signatures

```python
text_width(
    c: chr,  # the character to measure
    /,
) -> float

text_width(
    chars: list[chr],  # the character to measure
    start: int,  # first character to measure
    length: int,  # number of characters to measure
    /,
) -> float

text_width(
    str: str,  # the String of characters to measure
    /,
) -> float
```

Updated on March 06, 2023 02:49:26am UTC