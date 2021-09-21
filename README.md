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
Hello! Today we'll teach the Micro:bit to make its own decisions!

## Step 1 @showDialog
Up to this moment, all of our programs were following a single path and an only one sequence of actions, from start to finish. It's time to make our Micro:bit to behave a lot smarter by doing different things in different circumstances, making decisions.

To teach our Micro:bit to make decisions, we'll need the so called `conditional blocks` or `statements`.
```block
if (true) {
	
}
```
## Step 2 @showHint
### If statement block
An ``||logic.if||`` block runs the code inside only if the specified condition above is true. Let's add it to our code!
```block
if (true) {
	
}
```
## Step 3 @showDialog
Real-life examples of actions that can be expressed with an `If statement` logic:

- `If` it is raining outside, take an umbrella
- `If` you are hungry, have a dinner

Examples of robot decisions that can be written with an `if statement` logic:

- `If` a button is pressed, show a happy face
- `If` a robot is driving towards a wall, stop

Try to think of some other decisions that a human and a robot can make!

## Step 3 @showHint
### If statement block
Assemble the code as shown. The command to show a heart is inside the ``||logic.if||`` block, and the condition is `true`. Do you see the heart appear on screen?
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
Down below are some of the examples of them:  
  
```hint
3 is less than 5, so the condition is true.
```

```block
if(3<5){}
```
```hint
  
5 is not equal to 3, but a `not` block makes a false condition to become true.
Therefore, this condition is also true.
```
```block
if (!(5 == 3)){}
```
```hint
  
This condition becomes TRUE or FALSE randomly.
```
```block
if (Math.randomBoolean()){}
```
## Step 6 @showHint
### Writing conditions
Let's assemble our first code with conditions! We'll use the example from before: if the A-button is pressed, your Micro:bit will show a happy face!
```block
basic.forever(function () {
    if (input.buttonIsPressed(Button.A)) {
        basic.showIcon(IconNames.Happy)
    }
})
```
## Step 7 @showHint
### If-else statement block
An `If-else` statement block runs the first code if the specified condition above is true, otherwise runs the second code. 
You can find it inside the ``||logic.logic||`` category or turn an ``||logic.if||`` block into ``||logic.if else||`` by pressing ``||logic.+||``.
```block
if (true) {}
else{}
```
## Step 8 @showDialog
### If-else statement block
Let's rewrite our previous decisions with an `If-else statement` logic:

- If it is raining outside, take an umbrella, ELSE put on a hat
- If you are hungry, have a dinner, ELSE have a tea

Examples of robot decisions that can be written with an `If-else statement` logic:

- `If` a button is pressed, show a happy face, `else` show a sad face
- `If` a robot is driving towards a wall, stop, `else` go full-speed

## Step 9 @showHint
Now, let's change the code so that it uses an `If-else` statement. Do you notice that your Micro:bit shows a different face when you hold a button? Note that as you stop holding the button, the face changes back!
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
Now you know how to program Micro:bit to make decisions. Great! We will continue to use `if` and `if-else` statements in the next lessons.


