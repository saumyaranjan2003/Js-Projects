# INFO ABOUT THE PROJECTS

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