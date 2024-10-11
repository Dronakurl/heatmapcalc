# heatmapcalc

`heatmapcalc` is a Python package that provides a high-performance heatmap
calculation function implemented in Rust. This package leverages the power of
Rust for computationally intensive tasks while providing a simple and
easy-to-use Python interface.

## Features

- Efficient heatmap calculation using Rust
- Simple Python wrapper for easy integration

## Installation

You can then install the package using `pip`:

```sh
pip install heatmapcalc
```

If you have `setuptools` installed, you can also install the package using

```sh
pip install .
```

## Usage

Here is an example of how to use the `heatmapcalc` package:

```python
import numpy as np
from heatmapcalc import heatmapcalc

# Example detections: list of tuples (x1, y1, x2, y2)
detections = [(10, 10, 20, 20), (15, 15, 25, 25)]

# Shape of the heatmap
shape = (100, 100)

# Calculate the heatmap
heatmap = heatmapcalc(detections, shape)

# Display the heatmap
print(heatmap)
