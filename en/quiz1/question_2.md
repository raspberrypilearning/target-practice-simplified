
--- question ---
---
legend: Question 2 of 3
---

In your project, you used `if` , `elif`, and `else` conditions to check which colour the arrow landed on. 

In the example below, a variable called `speed` has the number `6` stored in it. When this `if` statement is run, what will be printed in the output area? 

--- code ---
---
language: python
---
speed = 6

if speed == 7:
    print('Super fast')
elif speed == 5:
    print('Pretty quick')
elif speed == 6:
    print('Very fast')
else:
    print('Speed not recognised!') 

--- /code ---

--- choices ---

- (x) `Very fast`

  --- feedback ---

  That's correct. The `speed` variable has been assigned the value `6`, which makes the `speed == 6` condition **True** so the program prints `Very fast`.

  --- /feedback ---

- ( ) `Speed not recognised!`

  --- feedback ---

  Not quite. Look at the value assigned to the `speed` variable.

  --- /feedback ---

- ( ) Nothing will be printed

  --- feedback ---
  
  Try again. `else` is used as a final option for when all the other conditions are false. Look through the conditions again. Are any of the conditions true?  

  --- /feedback ---

--- /choices ---

--- /question ---
