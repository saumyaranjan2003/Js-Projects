# SOME BRIEF INFORMATION ABOUT THE PROJECTS

1. **Calculator**: This project involves creating a basic calculator that can perform arithmetic operations such as addition, subtraction, multiplication, and division. Users can input numbers and operators to perform calculations.

2. **Color Scheme Switcher**: In this project, users can switch between different color schemes for the webpage. It provides buttons for selecting different colors, and upon clicking a button, the background color of the webpage changes accordingly.

3. **BMI Calculator**: This project calculates the Body Mass Index (BMI) of a person based on their height and weight input. BMI is a measure of body fat based on height and weight that applies to adult men and women. The calculator provides feedback on whether the user is underweight, normal weight, overweight, or obese based on their BMI value.

4. **Digital Clock**: The digital clock project involves creating a simple digital clock that displays the current time. It updates in real-time, showing the hours, minutes, and seconds. This project is a basic example of using JavaScript to manipulate the DOM and display dynamic content.

5. **Guess the Number**: This project is a simple number guessing game where the computer randomly selects a number and the user tries to guess it within a certain range. The game provides feedback on whether the user's guess is too high, too low, or correct. It's a fun way to practice basic programming concepts such as random number generation and conditional statements.
## PROJECT VIEW LINK 👇 HERE
[Click Here](link-add-Here)

## PROJECT-1
### Calculator
```javascript
```
## PROJECT-2
### Color Scheme Switcher
```javascript
const buttons = document.querySelectorAll(".button");

buttons.forEach(function(button) {
    button.addEventListener('click', function(e) {
        if (e.target.id === 'grey') {
            document.body.style.backgroundColor = 'grey';
        }
        if (e.target.id === 'white') {
            document.body.style.backgroundColor = 'white';
        }
        if (e.target.id === 'blue') {
            document.body.style.backgroundColor = 'blue';
        }
        if (e.target.id === 'yellow') {
            document.body.style.backgroundColor = 'yellow';
        }
    });
});


```

## PROJECT-3
### BMI Calculator
```javascript
const form = document.querySelector('form');
const nameInput = document.querySelector('#name');
const heightInput = document.querySelector('#height');
const weightInput = document.querySelector('#weight');
const result = document.querySelector('#result');

form.addEventListener('submit', function (e) {
    e.preventDefault();

    const name = nameInput.value.trim();
    const height = parseFloat(heightInput.value);
    const weight = parseFloat(weightInput.value);

    if (name === '') {
        result.innerHTML = "Please enter your name.";
    } else if (isNaN(height) || height <= 0 || heightInput.value === '') {
        result.innerHTML = "Please give a valid height.";
    } else if (isNaN(weight) || weight <= 0 || weightInput.value === '') {
        result.innerHTML = "Please give a valid weight.";
    } else {
        const bmi = (weight / ((height * height) / 10000)).toFixed(2);
        result.innerHTML = `<span>${name}, Your BMI is ${bmi}.</span>`;
    }
});
```

## PROJECT-4
### Digital Clock
```javascript
```

## PROJECT-5
### Guess the Number
```javascript
```