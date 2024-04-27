# Sum of squares
To further exploit the data, the scalar magnitudes r of the accelerometer and gyroscope were calculated. r is the scalar magnitude of the three combined data points: x, y, and z. The advantage of using r versus any particular data direction is that it is impartial to device orientation and can handle dynamic re-orientations. r is calculated by:
```
r_{magnitude} = \sqrt{x^2 + y^2 + z^2}
```