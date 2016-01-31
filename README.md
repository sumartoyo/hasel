python+numpy RGB to HSL (and vice versa) converter

```python
import matplotlib.image as mpimg
import hasel

image = mpimg.imread('image.jpg')

hsl = hasel.rgb2hsl(image)
# input: numpy array, shape: (height, width, 3), dtype: uint8 [0, 255]
# output: numpy array, shape: (height, width, 3), dtype: float [0.0, 1.0)

rgb = hasel.hsl2rgb(hsl)
# input: numpy array, shape: (height, width, 3), dtype: float [0.0, 1.0)
# output: numpy array, shape: (height, width, 3), dtype: uint8 [0, 255]
```
