# turing (on the spot)
right
```
def right():
    go(100, -100, 0.76)
```
left
``` 
def left():
    go(-100, 100, 0.76)
```
# turning (move backwards)
right
```
def right():
    go(-90, 20, 1.3)
```
left
```
def left():
    go(20, -90, 1.3)
```
# turning (move forwards)
right
```
def right():
    go(100, 10, 1.55)
```
left
```
def left():
    go(10, 100, 1.55)
```
# sensors
color
```
get_color()[0][0]
```
ultrasound
```
get_ultrasound()[0]
```
# loops
for loops
```
for i in range(4):
    #code here
```
while loops
```
while i < 4:
    #code here
    i += 1
```
# collect data
get angle
```
print('angle:', angle())
```
format value
```
# Example floating-point number
number = 123.456789

# Using format() with .2f to format the number to two decimal places
formatted_number = "{:.2f}".format(number)

# Printing the formatted number
print(formatted_number)
```
# shape drawing
infinity loop
```
go(-50, 50, 2)
go(100, 1, 4)
go(50, 50, 1.5)
go(1, 100, 4.1)
go(50, 50, 1.6)
```
tripod turn
```
go(50, 50, 2)
go(25, 90, 2)
go(-45, -45, 2.5)
go(25, 90, 2)
go(50, 50, 2)
```
triangle
```
set(200,700,1)
go(25,-25,1)
go(70,70,3.5)
go(87,-87,1)
go(70,70,3.5)
go(87,-87,1)
go(70,70,3.5)
```
trace centre
```
left_speed = 50
right_speed = 50
while active():
    if get_intensity()[0] > 0:
        left_speed = -100
        right_speed = 100
    elif get_intensity()[3] > 0:
        left_speed = 100
        right_speed = -100
    elif get_intensity()[1] > 0:
        left_speed = 80
        right_speed = 100
    elif get_intensity()[2] > 0:
        left_speed = 100
        right_speed = 80
```
number 5
```
set(700,400,0)
go(-100,100,0.7)
go(100,100,1)
go(-100,100,0.7)
go(100,100,0.5)
go(-100,100,0.7)
go(100,100,0.8)
go(100,-10,2.5)
go(100,100,0.9)
```
number 6
```
set(500,200,0)
go(-100,100,1)
go(50,100,2.3)
go(1,100,4.6)
```
semicircle arc
```
set(500,170,270)
go(40,90,5.4)
```
# things to note
intensity
```
Intensity = R + G + B divide by 3
```
Funtions
```
while active():
```
