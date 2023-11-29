## Add more conditions

`elif` (else - if) can be used to add more conditions to your `if` statement. These will be read from top to bottom. As soon as a **True** condition is found, it will be actioned. Any remaining conditions will be ignored.

--- task ---

Score points if the arrow lands on the `inner` or `middle` circles 🎯: 

--- code ---
---
language: python
line_numbers: true
line_number_start: 6
line_highlights: 9-12
---

def mouse_pressed():
    if hit_colour == Color('blue').hex:   
        print('You hit the outer circle, 50 points!')
    elif hit_colour == Color('red').hex:
        print('You hit the inner circle, 200 points!')
    elif hit_colour == Color('yellow').hex:
        print('You hit the middle, 500 points!')

--- /code ---

--- /task ---

--- task ---

**Test:** 🔄 Run your project. Try to fire the arrow on the inner and middle circles to see the messages.

![An arrow touching the inner circle of the target in the Visual Output area. The points message is displayed in the Text Output area.](images/yellow-points.png)

--- /task ---

--- collapse ---

---
title: Debug your code
---

+ Check that your indentation matches the example.

+ If you see a message about `hit_colour` being "not defined", go back to `shoot_arrow()` and check the line that declares `hit_colour` as a global variable.

+ Make sure you have entered the correct colour names for your circles. 

+ Make sure you have used the `.hex` string for your circle colours.

--- /collapse ---

### Missing the target

There is one more decision you need to make: what happens if the arrow does not land on any of the target circles? ❌ 

To do this last check, you use `else`.

--- task ---

Add code to `print()` a message `else` none of the `if` and `elif` conditions have been met.

--- code ---
---
language: python
line_numbers: true
line_number_start: 6
line_highlights: 13-14
---

def mouse_pressed():
    if hit_colour == Color('blue').hex:   
        print('You hit the outer circle, 50 points!')
    elif hit_colour == Color('red').hex:
        print('You hit the inner circle, 200 points!')
    elif hit_colour == Color('yellow').hex:
        print('You hit the middle, 500 points!')
    else:   
        print('You missed! No points!')

--- /code ---

--- /task ---

--- task ---

**Test:** 🔄 Run your project. Fire the arrow in the grass or sky to see the miss message. 

**Choose:** 💭 Change the number of points scored for hitting the different circles.

--- /task ---

--- save ---