## Get the colour hit by the arrow 

The `get()` function returns the colour of a pixel.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
A <span style="color: #0faeb0; font-weight: bold;">pixel</span>, short for picture element, is a single coloured dot within an image. Images are made up of lots of coloured pixels.
</p>

--- task ---

Add a **global variable** called `hit_colour` that can be used throughout your code.

Add code to `get` the colour of the pixel at the centre of the arrow and store it in the `hit_colour` variable. 
In order to compare the colours, we need to use the hexadecimal code this can be done with the `.hex` string.

--- code ---
---
language: python
line_numbers: true
line_number_start: 7
line_highlights: 8, 11
---
# The shoot_arrow function goes here     
def shoot_arrow():
    global hit_colour  # Can be used in other functions  
    arrow_x = randint(100, 300)  # Store a random number between 100 and 300    
    arrow_y = randint(100, 300)  # Store a random number between 100 and 300
    hit_colour = get(arrow_x, arrow_y).hex  # Get the hit colour     
    fill('sienna')  # Set the arrow to fill colour to brown   
    circle(arrow_x, arrow_y, 15)  # Draw a small circle at random coordinates
  
--- /code ---

**Tip:** 💡 The code to `get` the colour needs to be **before** the code to draw the `circle` otherwise you will always save the wood colour of the arrow! 

--- /task ---

### Print the colour when the mouse is pressed

The `p5` library 'listens' for certain events, one of these is the press of the mouse button. When it detects that the button has been pressed, it will run whatever code it has been given in the `mouse_pressed` function.

--- task ---

Define your `mouse_pressed()` function under the comment **# The mouse_pressed function goes here**. 

Add code to print the target emoji 🎯 when the mouse is clicked.

--- code ---
---
language: python
line_numbers: true
line_number_start: 5
line_highlights: 6
---

# The mouse_pressed function goes here    
def mouse_pressed():    
    print('🎯')

--- /code ---

--- /task ---

--- task --- 

**Test:** 🔄 Run your project. 

The project prints 🎯 each time the arrow is redrawn.

![An animation of target with a brown circle arrow appearing in a variety of positions.](images/fire_arrow.gif)

**Debug:** 🐞 If you are seeing a message about `hit_colour` being 'not defined', then go back to `shoot_arrow()` and check that you have included the `global hit_colour` line.

**Debug:** 🐞 Check the `print` line really carefully for commas and brackets. 

--- /task ---

--- save ---
