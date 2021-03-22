# Building-blocks-js from MDN


- [X] [Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)
- [ ] [looping code](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code)
- [ ] [Functions -reusables blocks](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)
- [ ] [Your own function](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Build_your_own_function)
- [ ] [Function return value](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Return_values)
- [ ] [Introduct to event](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

## Conditionals 

- The code needs to make decisions and carry out actions accordingly depending on different inputs. 
- Conditional statements allow us to represent such decision making in JavaScript, from the choice that must be made (for example, "one cookie or two"), to the resulting outcome of those choices (perhaps the outcome of "ate one cookie" might be "still felt hungry",...)
- if..else statements : definition, A note on comparison operators, Nesting if ... else, Logical operators: AND, OR and NOT
- switch statements: switch, case, break, default
- ternary operator: white and black website. 

#### More color choices! 

```

<!DOCTYPE html>
<html>
<body>

<label for="theme">Select theme: </label>
<select id="theme">
  <option value="white">White</option>
  <option value="black">Black</option>
  <option value="purple">Purple</option>
  <option value="yellow">Yellow</option>
  <option value="psychedelic">psychedelic</option>
  
</select>

<h1>This is the website color</h1>

<script>

const select = document.querySelector('select');
const html = document.querySelector('html');

select.onchange = function() {
 const choice = select.value;

 switch(choice) {
 case 'black':
 update('black','white');
 break;
 case 'white':
 update('white','black');
 break;
 case 'purple':
 update('purple','white');
 break;
 case 'yellow':
 update('yellow','darkgray');
 break;
 case 'psychedelic':
 update('lime','purple');
 break;
 }
}

function update(bgColor, textColor) {
 html.style.backgroundColor = bgColor;
 html.style.color = textColor;
}
 

</script>

</body>
</html>
```
## Looping code

- A loop has one or more of these features: 
1. counter: inizialited with certain value, like I don't have food and I need to reach this amount. 
2. condition : when the loop needs to stop, Have I got enough food?. If yes! stop!
3. iterator: which generally increments the counter by a small amount on each successive loop until the condition is no longer "true". 

```
loop(food = 0; foodNeeded = 10) {
  if (food >= foodNeeded) {
    exit loop;
    // We have enough food; let's go home
  } else {
    food += 2; // Spend an hour collecting 2 more food
    // loop will then run again
  }
}
```
- For Loop : 
The keyword for, followed by some parentheses.
1. initializer: this is usually a variable set to a number, que se incrementa para contar el número de veces que se ha ejecutado el bucle. A veces también se la denomina counter variable.  
2. condition: when needs to stop
3. final expression:  this is always evaluated (or run) each time the loop has gone through a full iteration.

```

const cats = ['Bill', 'Jeff', 'Pete', 'Biggles', 'Jasmin'];
let info = 'My cats are called ';
const para = document.querySelector('p');

for (let i = 0; i < cats.length; i++) {
  info += cats[i] + ', ';
}

para.textContent = info;

```
Important: With for — as with all loops — you must make sure that the initializer is incremented or, depending on the case, decremented, so that it eventually reaches the point where the condition is not true. If not, the loop will go on forever, and either the browser will force it to stop, or it will crash. This is called an infinite loop.

- While Loop

1. Inizializer is set before the loop. 
2. And final-expression is inside the loop after code runs.
3. Condition is included in the parentheses, which is preceded by while keyword. 

```
initializer
while (condition) {
  // code to run

  final-expression
}

```
   - do...while
  There is a variation in while structure
  
  ```
  initializer
do {
  // code to run

  final-expression
} while (condition)


```
