## Create a background

<div style="display: flex; flex-wrap: wrap">
<div>

![The output area with a sky-coloured rectangle above a grass-coloured rectangle to create the background.](images/background.png){:width="300px"}

</div>
</div>

### Open the starter project

--- task ---

Open the [Target practice starter](https://editor.raspberrypi.org/en/projects/target-practice-starter){:target="_blank"} project. The code editor will open in another browser tab.

If you have a Raspberry Pi account, click on the **Save** button to save a copy to your **Projects**.

--- /task ---

### Edit the sky

--- task ---

The starter project has code already written for you. 

Click **'Run'** to see a blue filled rectangle which is the sky in your project. 

![A blue rectangle with a black border around it, above a grey rectangle. The top left corner of the canvas is marked as x=0, y=0 this is the origin of the rectangle. The width is highlighted as 400 and the height as 250. The code rect(0, 0, 400, 250) is shown.](images/sky_stroke.png){:width="400px"}

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
# Setup your game here
    size(400, 400)  # Width and height of screen
    no_stroke()

--- /code ---

--- /task ---

--- task ---

**Run** your code again and notice 👀 that the border (stroke) has now disappeared.

**Tip:** 💡 You will need to press **Stop** to stop your program, this will make the **Run** button reappear. 

**Tip:** 💡 Coordinates start from (x=0, y=0) in the top left corner. This might be different to other coordinate systems you have used. 

--- /task ---