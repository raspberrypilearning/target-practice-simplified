## Draw the grass

--- task ---

**Add** code to draw a green rectangle at the bottom of the screen.

![The output area with a sky-coloured rectangle above a grass-coloured rectangle to create the background. The top left corner of the rectangle is marked as x=0, y=250 this is the origin of the rectangle. The width is highlighted as 400 and the height as 150. The code rect(0, 250, 400, 150) is shown.](images/green-grass.png){:width="400px"}

--- code ---
---
language: python
filename: main.py — draw()
line_numbers: true
line_number_start: 14
line_highlights: 18-19
---
def draw():
# Things to do in every frame
    fill('cyan')  # Set the fill colour for the sky to cyan
    rect(0, 0, 400, 250)  # Draw a rectangle for the sky with these values for x, y, width, height
    fill('lightgreen')  # Set the fill colour for the grass to light green
    rect(0, 250, 400, 150)  # Draw a rectangle for the grass with these values for x, y, width, height

--- /code ---

**Tip:** 💡 We have added comments to our code, like `# Set the fill colour for the sky to cyan`, to tell you what it does. You don't need to add comments to your code, but they are helpful to remind you what lines of code do.

--- /task ---

--- task ---

**Test:** 🔄 Run your project again to view the finished background. 

![The output area with a sky-coloured rectangle above a grass-coloured rectangle to create the background.](images/background.png){:width="400px"}

--- /task ---

--- save ---