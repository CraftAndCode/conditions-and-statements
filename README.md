# Conditions and statements

```package
core
radio
microphone
```

```template
basic.forever(function () {
    
})
```

```blocks
basic.forever(function () {
    
})
```
## Step 0 @showDialog
Hello! Today we're going to teach the Micro:bit to make its own decisions!

## Step 1 @showDialog
Until now, all  programs followed a single path and only one sequence of actions, from start to finish. It's time to make our Micro:bit behave smarter by doing different things in different circumstances - making decisions.

To teach our Micro:bit to make decisions, we'll need so-called `conditional blocks` or `statements`.
```block
if (true) {
    
}
```
## Step 2 @showHint
### If statement block
An ``||logic.if||`` block runs the code inside only if the  condition specified above is true. Let's add it to our code!
```block
if (true) {
    
}
```
## Step 3 @showDialog
Real-life examples of actions that can be expressed with an `If statement` logic:

- `If` it is raining outside, take an umbrella
- `If` you are hungry, have something to eat

Examples of robot decisions that can be written with an `if statement` logic:

- `If` a button is pressed, show a happy face
- `If` the robot is driving towards a wall, stop

Try to think of some other decisions that a human and a robot can make!

## Step 3 @showHint
### If statement block
Assemble the code as shown. The command to show a heart is inside the ``||logic.if||`` block, and the condition is `true`. Do you see the heart on screen?
```blocks
if (true) {
    basic.showIcon(IconNames.Heart)
}
```

## Step 4 @showHint
### If statement block
Now, let's switch the condition to be `false`. Does the heart appear now?
```blocks
if (false) {
    basic.showIcon(IconNames.Heart)
}
```

## Step 5 @showDialog
### Writing conditions
Conditions are hexagonal blocks that you can put inside the slot of ``||logic.if||`` blocks and they can be either `TRUE` or `FALSE`. They are just like equations that can be correct or not correct!  
Below are some  examples of these:  
  
```hint
3 is less than 5, so the condition is true.
```

```block
if(3<5){}
```
```hint
  
5 is not equal to 3, but a `not` block makes a false condition become true.
Therefore, this condition is also true.
```
```block
if (!(5 == 3)){}
```
```hint
  
This condition becomes TRUE or FALSE at random.
```
```block
if (Math.randomBoolean()){}
```
## Step 6 @showHint
### Writing conditions
Let's assemble our first code with conditions! We'll use the example from earlier: if the A button is pressed, your Micro:bit will show a happy face!
```block
basic.forever(function () {
    if (input.buttonIsPressed(Button.A)) {
        basic.showIcon(IconNames.Happy)
    }
})
```
## Step 7 @showHint
### If-else statement block
An `If-else` statement block runs the first code if the specified condition above is true, otherwise it runs the second code. 
You can find it inside the ``||logic.logic||`` category or turn an ``||logic.if||`` block into ``||logic.if else||`` by pressing ``||logic.+||``.
```block
if (true) {}
else{}
```
## Step 8 @showDialog
### If-else statement block
Let's rewrite our earlier examples with `If-else statement` logic:

- If it is raining outside, take an umbrella, ELSE put on a hat
- If you are hungry, have something to eat, ELSE have tea

Examples of robot decisions that can be written with an `If-else statement` logic:

- `If` a button is pressed, show a happy face, `else` show a sad face
- `If` the robot is driving towards a wall, stop, `else` proceed at full speed

## Step 9 @showHint
Now, let's change the code so that it uses an `If-else` statement. Did you notice that your Micro:bit displays a different face when you hold the button? Note that when you stop holding the button, the face changes back!
```blocks
basic.forever(function () {
    if (input.buttonIsPressed(Button.A)) {
        basic.showIcon(IconNames.Happy)
    } else {
        basic.showIcon(IconNames.Sad)
    }
})
```
## Step 10
Now you know how to program he Micro:bit to make decisions. Great! We will continue to use `if` and `if-else` statements in the next lesson.
