# Projects related to DOM

## project link
[Click here](https://stackblitz.com/edit/dom-project-chaiaurcode?file=index.html)

# Solution code

## Project 1

```javascript
const buttons = document.querySelectorAll('.button');
const body = document.querySelector("body")

buttons.forEach(function(button){
  console.log(button)
  button.addEventListener('click', function(e){
   console.log(e)
   console.log(e.target) //event aa kaha se rha hai-->e.target
   if(e.target.id === 'grey'){
     body.style.background = e.target.id;
   }
   if(e.target.id === 'white'){
     body.stlye.background = e.target.id;
   }
   if(e.target.id === 'blue'){
    body.stlye.background = e.target.id;
  }
  if(e.target.id === 'yellow'){
    body.stlye.background = e.target.id;
  }
  })
})
```

## Project 2

```javascript
const form = document.querySelector('form');
//const height = parseInt(document.querySelector('#height').value)
//this usecase will give empty value.
form.addEventListener('submit', function (e) {
  e.preventDefault();
  const height = parseInt(document.querySelector('#height').value);
  const weight = parseInt(document.querySelector('#weight').value);
  if (height === '' || height < 0 || isNaN(height)) {
    results.innerHTML = `Please give a valid height ${height}`;
  } else if (weight === '' || weight < 0 || isNaN(weight)) {
    results.innerHTML = `Please give a valid weight ${weight}`;
  } else {
    const bmi = (weight / ((height * height) / 10000)).toFixed(2);
    //show the result
    results.innerHTML = `<span>${bmi}</span>`;
  }
});

```

## Project 2

```javascript
const clock = document.getElementById('clock');
// const clock = document.querySelector('#clock')

setInterval(function () {
  let date = new Date();
  // console.log(date.toLocaleTimeString());
  clock.innerHTML = date.toLocaleTimeString();
}, 1000);


```
## Project 3

```javascript

```