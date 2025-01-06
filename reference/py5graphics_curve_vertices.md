# Py5Graphics.curve_vertices()

Create a collection of curve vertices.

## Description

Create a collection of curve vertices. The purpose of this method is to provide an alternative to repeatedly calling [](py5graphics_curve_vertex) in a loop. For a large number of curve vertices, the performance of `curve_vertices()` will be much faster.

The `coordinates` parameter should be a numpy array with one row for each curve vertex.  There should be two or three columns for 2D or 3D points, respectively.

This method is the same as [](sketch_curve_vertices) but linked to a `Py5Graphics` object. To see example code for how it can be used, see [](sketch_curve_vertices).

## Signatures

```python
curve_vertices(
    coordinates: Iterator[Iterator[float]],  # 2D array of curve vertex coordinates with 2 or 3 columns for 2D or 3D points, respectively
    /,
) -> None
```

Updated on January 06, 2025 22:21:18pm UTC
