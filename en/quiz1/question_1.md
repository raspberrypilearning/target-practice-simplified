## Quick quiz

Answer the three questions. There are hints to guide you to the correct answer.

When you have answered each question, click on **Check my answer**.

Have fun!

--- question ---
---
legend: Question 1 of 3
---
In your project, you added `no_stroke()` to your `setup()` function. What does the `no_stroke()` function do?

--- code ---
---
language: python
---

def setup():   
  size(400, 400)      
  no_stroke()  
  
--- /code ---

--- choices ---

- ( ) It draws a shape using the coordinates given.

  --- feedback ---

Not quite. In this example, the `size()` function does this.

  --- /feedback ---

- ( ) It fills the shape with a given colour.

  --- feedback ---

Not quite. The `fill()` function does this and will usually include a given colour.

  --- /feedback ---

- (x) It turns off the border (stroke) for all the shapes.

  --- feedback ---

  That's correct. If you do not use this function, a black border will be drawn around your shapes.

  --- /feedback ---

- ( ) It draws a circle shape.

  --- feedback ---

  Not quite. The `circle()` function would be used to draw a circle.

  --- /feedback ---

--- /choices ---

--- /question ---
