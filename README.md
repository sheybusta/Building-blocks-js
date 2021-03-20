# Building-blocks-js from MDN


- [X] [Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)
- [ ] [looping code](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code)
- [ ] [Functions -reusables blocks](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)
- [ ] [Your own function](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Build_your_own_function)
- [ ] [Function return value](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Return_values)
- [ ] [Introduct to event](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

### Conditionals 

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
