# Building-blocks-js from MDN


- [ ] [Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)
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

##### A simple calendar example:
- In this example, you are going to help us finish a simple calendar application. In the code you've got:

- A <select> element to allow the user to choose between different months.
- An onchange event handler to detect when the value selected in the <select> menu is changed.
- A function called createCalendar() that draws the calendar and displays the correct month in the ... element.

- We need you to write a conditional statement inside the onchange handler function, just below the // ADD CONDITIONAL HERE comment. It should:

- Look at the selected month (stored in the choice variable. This will be the <select> element value after the value changes, so "January" for example.)
 - Set a variable called days to be equal to the number of days in the selected month. To do this you'll have to look up the number of days in each month of the     year. You can ignore leap years for the purposes of this example.
- Hints:

- You are advised to use logical OR to group multiple months together into a single condition; many of them share the same number of days.
- Think about which number of days is the most common, and use that as a default value.
