## Fire your arrow

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
When you click or tap, an arrow will fire at the position of a moving target circle. 
</div>
<div>

![The target, with a brown circle arrow appearing in a variety of positions.](images/fire_arrow.gif){:width="300px"}

</div>
</div>

### Draw a target circle every frame

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;"> Computers create the effect of movement by showing lots of images one after another. Each image is called a <span style="color: #0faeb0; font-weight: bold;"> frame </span>.   
</p>

--- task ---

Define your `shoot_arrow()` function under the comment **# The shoot_arrow function goes here**. 

Add code to randomly draw a brown circle within a target area:

![A rectangle showing the target area coordinates in a semi transparent rectangle. The target area is between x=100 and y=100 to x=300 and y=300 so covers the whole target and wider.](images/target_area.png)

--- code ---
---
language: python
filename: main.py — shoot_arrow()
line_numbers: true
line_number_start: 7
line_highlights: 8-12
---
# The shoot_arrow function goes here    
def shoot_arrow():   
    arrow_x = randint(100, 300)  # Store a random number between 100 and 300    
    arrow_y = randint(100, 300)  # Store a random number between 100 and 300    
    fill('sienna')  # Set the arrow to fill colour to brown   
    circle(arrow_x, arrow_y, 15)  # Draw a small circle at random coordinates

--- /code ---

--- /task ---

--- task ---

Go to the `draw` function and call your new `shoot_arrow` function. 

--- code ---
---
language: python
filename: main.py — draw()
line_numbers: true
line_number_start: 31
line_highlights: 33
---
    fill('yellow')  # Set the colour for the circle fill to yellow      
    circle(200, 200, 30)  # Draw the middle circle using x, y, width
    shoot_arrow()

--- /code ---

--- /task ---

--- task ---

**Test:** 🔄 Run your code and see the arrow appear in a random position each frame.

![An animation of target with a brown circle arrow appearing in a variety of positions.](images/fire_arrow.gif)

The background and target will be drawn over the old arrow. This means you only see one arrow at a time.

--- /task ---

