python+numpy RGB ↔ HSL converter  
*a study of numpy and threading*

```python
import matplotlib.image as mpimg
import hasel.color as hc

image = mpimg.imread('image.jpg')

hsl = hc.rgb2hsl(image)
# input: numpy array, shape: height*width*3, dtype: uint8 [0, 255]
# output: numpy array, shape: height*width*3, dtype: float [0.0, 1.0)

rgb = hc.hsl2rgb(hsl)
# input: numpy array, shape: height*width*3, dtype: float [0.0, 1.0)
# output: numpy array, shape: height*width*3, dtype: uint8 [0, 255]
```
