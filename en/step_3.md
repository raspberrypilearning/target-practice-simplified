## Draw the grass

--- task ---

**Add** the code to draw a green rectangle at the bottom of the screen.

![A background made up of a sky-coloured rectangle above a grass-coloured rectangle. The top left-hand corner of the green rectangle is marked as x=0, y=250. The width is highlighted as 400 and the height as 150. Above the green rectangle, the code rect(0, 250, 400, 150) is shown.](images/green-grass.png){:width="400px"}

--- code ---
---
language: python
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

--- /task ---

--- collapse ---

---
title: Comments
---
**Tip:** 💡 Comments are useful because they remind you what lines of code do. We have added comments to our code, like `# Set the fill colour for the sky to cyan`, to tell you what the code does.

--- /collapse ---

--- task ---

**Test:** 🔄 Run your project again to see the full background.

![A background made up of a sky-coloured rectangle above a grass-coloured rectangle.](images/background.png){:width="400px"}

--- /task ---

--- save ---