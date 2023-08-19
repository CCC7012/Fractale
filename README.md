# Fractale
Une fractale / A fractal


```python
from turtle import *

def carre(lg) :
    if lg >= 1 :
        forward(lg/2)
        right(135)
        carre(lg/3)
        right(135)
        for loop in range(3) :
            forward(lg)
            right(135)
            carre(lg/3)
            right(135)
        forward(lg/2)

penup()
speed(99999999)
goto(0,-50)
pendown()
carre(200)
exitonclick()
