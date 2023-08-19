# Fractale
Une fractale / A fractal


### Result




### Code
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

title("Fractale")
penup()
speed(0)
goto(0,-50)
pendown()
carre(200)
exitonclick()
