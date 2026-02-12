# python-practice
Python practice is a demo git repo for my beginner level codes in python



# Hurdle 4 puzzle solution for Reeborg's World in python
def turn_right():
    turn_left()
    turn_left()
    turn_left()
    
def jump():    
    turn_left()
    while wall_on_right():
        move()
    turn_right()
    move()
    turn_right()
    while front_is_clear():
        move()
    turn_left()
    
while not at_goal():
    if wall_in_front():
        jump()
    elif front_is_clear():
        move()
