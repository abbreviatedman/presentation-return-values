@snap[north]
## Return Values 101
#### From Code Immersives
@snapend

@snap[south]
![](https://www.codeimmersives.com/wp-content/uploads/2019/09/cropped-CodeImmersives_Logo_RGB_NYC_BW-3.png)
@snapend

---

@snap[north]
## The Final Function Technique
@snapend

@snap[south]
![](https://media.moddb.com/images/downloads/1/60/59795/return_6.jpg)
@snapend
---

## What's `return` FOR?

Parameters let us give input to our functions; **`return`** gives us output!

![](http://pluspng.com/img-png/input-output-machine-png-asynchronous-1600.png)

---

## How's It Work?

@snap[code-noblend]
```javascript
function exclaim(greeting) {
  const yelled = greeting + '!';

  return yelled;
}
```
@snapend

Whatever is immediately after **`return`** becomes the output of our function!

---

### Now We Can USE That Output

@snap[code-noblend]
```javascript
function exclaim(greeting) {
  const yelled = greeting + '!';

  return yelled;
}

const yelledGreeting = exclaim('Hi');
yelledGreeting; // -> 'Hi!'
```
@snapend

---

### Our Functions Evaluate Now

The "return value" is whatever *we decide* the function evaluates to.

@snap[code-noblend]
```javascript
const yelledGreeting = exclaim('Hi');
```
@snapend

**`exclaim('Hi')`** evaluates to **`'Hi!'`** according to our function, so we can take that value and put it in a variable!

---

## Now Instead Of This:

@snap[code-noblend]
```javascript
let x = 3;

function add5() {
  x = x + 5;
}
```
@snapend

---

## We Can Do This:

@snap[code-noblend]
```javascript
const x = 3;
const y = 15;

function add5(num) {
  return num + 5;
}

const bumpedX = add5(x);
const bumpedY = add5(y);

bumpedX; // -> 8
bumpedY; // -> 20
```
@snapend

---

## All Functions Return SOMETHING

But if you don't explicitly return, JavaScript returns **`undefined`** for you.

@snap[code-noblend]
```javascript
function whoopsForgotToReturn(x, y) {
  const sum = x + y;
}

const oopsie = whoopsForgotToReturn(5, 15);

oopsie; // -> undefined
```
@snapend

---
@snap[north span-100]
## Now You Have... **`return`**!!!
@snapend

@snap[south]
![](https://thumbs.gfycat.com/FaithfulLawfulKusimanse-max-1mb.gif)
@snapend