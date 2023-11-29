## Create a background

<div style="display: flex; flex-wrap: wrap">
<div>

![A background made up of a sky-coloured rectangle above a grass-coloured rectangle.](images/background.png){:width="300px"}

</div>
</div>

### Open the starter project

--- task ---

Open the [Target practice starter project](https://editor.raspberrypi.org/en/projects/target-practice-starter){:target="_blank"}. The Code Editor will open in another browser tab.

If you have a Raspberry Pi account, click the **Save** button to save a copy to your **Projects**.

--- /task ---

### Edit the sky

--- task ---

The starter project has code that has already been written for you. 

Click on **Run** to see a blue-filled rectangle, which is the sky in your project.

![A blue rectangle with a black border around it, above a grey rectangle. The top left-hand corner of the blue rectangle is marked as x=0, y=0. The width is highlighted as 400 and the height as 250. Below the blue rectangle, the code rect(0, 0, 400, 250) is shown.](images/sky_stroke.png){:width="400px"}

--- /task ---

--- task ---

The sky has been drawn with a black border (stroke). 

Turn the stroke off for all shapes. Add `no_stroke()` to the `setup` function:

--- code ---
---
language: python
line_numbers: true
line_number_start: 9
line_highlights: 12
---
def setup():
# Set up your game here
    size(400, 400)  # width and height of screen
    no_stroke()

--- /code ---

--- /task ---

--- task ---

**Run** your code again. Did you notice 👀 that the border (stroke) has now disappeared?

--- /task ---
--- collapse ---

---
title: Tips on coordinates and running your program
---

To stop your program, you need to press **Stop**. This will make the **Run** button reappear.

Coordinates start from (x=0, y=0) in the top left-hand corner. This might be different to other coordinate systems you have used.

--- /collapse ---