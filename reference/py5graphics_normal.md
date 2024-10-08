# Py5Graphics.normal()

Sets the current normal vector.

## Description

Sets the current normal vector. Used for drawing three dimensional shapes and surfaces, `normal()` specifies a vector perpendicular to a shape's surface which, in turn, determines how lighting affects it. Py5 attempts to automatically assign normals to shapes, but since that's imperfect, this is a better option when you want more control. This function is identical to `gl_normal3f()` in OpenGL.

This method is the same as [](sketch_normal) but linked to a `Py5Graphics` object. To see example code for how it can be used, see [](sketch_normal).

Underlying Processing method: PGraphics.normal

## Signatures

```python
normal(
    nx: float,  # x direction
    ny: float,  # y direction
    nz: float,  # z direction
    /,
) -> None
```

Updated on March 06, 2023 02:49:26am UTC
