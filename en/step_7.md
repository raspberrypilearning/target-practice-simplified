## Score points

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Your game will add scores based on where the arrow hits.
</div>
<div>

![An animation of the target, with the arrow appearing in a variety of positions, and scores appearing as text below the game.](images/points-scored.gif){:width="300px"}

</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
We use <span style="color: #0faeb0; font-weight: bold;"> conditions</span> all the time to make decisions. We could say 'if the pencil is blunt, then sharpen it'. Similarly, `if` conditions let us write code that do something different depending on whether a condition is true or false.
</p>

### Display the scores

--- task ---

Delete ❌ the `print('🎯')` line of code.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 5
line_highlights: 7
---
# The mouse_pressed function goes here    
def mouse_pressed():


--- /code ---

--- /task ---

--- task ---

Display a message **if** the `hit_colour` is equal to the `outer` circle colour (blue) 🎯. 

Notice 👀 that the code uses two equals signs `==` to mean **equal to**.

--- code ---
---
language: python
filename: main.py - mouse_pressed()
line_numbers: true
line_number_start: 5
line_highlights: 7, 8
---

# The mouse_pressed function goes here     
def mouse_pressed():     
    if hit_colour == Color('blue'):  # Like the code in functions, the code in 'if' statements is indented
        print('You hit the outer circle, 50 points!')

--- /code ---

**Tip:** 💡 If you changed the colour of your outer circle then you will need to replace `'blue'` with the colour name that you have chosen.

--- /task ---

--- task ---

**Test:** 🔄 Run your project. Try to fire the arrow on the blue outer circle to see the message. 

**Tip:** 💡 `frame_rate=2`, in `run` at the bottom of your code, controls how fast your game draws. If it's going too fast, set it to a lower number. 

![The output area with arrow touching the outer circle. The points message is displayed in the output area.](images/blue-points.png)

**Debug:** 🐞 Check that you have used the American spelling of 'Color' (without a 'u') and that 'Color' is capitalised.

**Debug:** 🐞 Make sure your code matches exactly and you indented the code inside your `if` statement. 

**Debug:** 🐞 Make sure that you have entered the correct colour name you used for **your** outer circle. 

--- /task ---
