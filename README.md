# Le Wagon Prep: JavaScript

## Exercise 1:

Write a JS script that logs in the console if you can vote or not depending on your age. Improve this script by adding the condition that if you are more than 21, you can be elected as President.

### Solution

```js
function electionCheck(age) {
    if(age >= 21) {
        console.log(“you can run for president”);
    } else if(age >= 18) {
        console.log(“you can vote”);
    } else {
        console.log(“you’re too young to participate in the election”);
    }
}

electionCheck(10); // “you’re too young to participate in the election”
electionCheck(18); // “you can vote”
electionCheck(21); // “you can run for president”
```

## Exercise 2:

Write a JS script that iterates over the IMDB list of 10 top rated movies and then prints each title.

### Solution

```js
// CSS selectors valid as of May 2021 on https://www.imdb.com/chart/top/?ref_=nv_mv_250

// select all title elements
const titleCol = document.querySelectorAll(‘.titleColumn’)

// loop through and log all 250
titleCol.forEach(title => console.log(title.querySelector(‘a’).innerText))

// loop and log top 10 only
for(let i=0; i<10; i++) {
console.log(titleCol[i].querySelector(‘a’).innerText);
}
```

## Exercise 3:

Go to Le Wagon website and hide/show the logo. Then make it green.

### Solution

```js
// CSS selectors valid as of May 2021
document.querySelector(‘.navbar__logo’).style.display = ‘none’
```
