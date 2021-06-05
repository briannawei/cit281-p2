## Project 2

<img width="1680" alt="p2-vsCode-diff" src="https://user-images.githubusercontent.com/84175061/120882246-311c5b00-c58b-11eb-92a6-71836c349771.png">
[p2-random-files.txt](https://github.com/briannawei/cit281-p2/files/6602100/p2-random-files.txt)
[p2-random-commits.txt](https://github.com/briannawei/cit281-p2/files/6602101/p2-random-commits.txt)


### p2-expressions.js
```
/*
    CIT 281 Project 2
    Name: Brianna Wei
*/

// Returns a random number between min (inclusive) and max (exclusive)
const getRandomInteger = function(min, max) { return Math.floor(Math.random() * (max - min) + min);}

// Canvas posted solution for project 1
const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
let result = "";

for (let i = 0; i < getRandomInteger(5, 26); i++) {
    result += alphabet[getRandomInteger(1,alphabet.length-1)];
}

console.log(getRandomString(10,20));

// Return a single, random, lowercase letter
const getRandomLetter = function() {const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
    let randomLetter = getRandomInteger(0,25);
    return alphabet[randomLetter];
}

// Return the random length string
const getRandomString = function(minLength,maxLength) {let result = "";
    const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
    let randomChar = getRandomInteger(minLength,maxLength);
    for (let i=0; i < randomChar; i++) {
        result = result + getRandomLetter();
    }
    console.log(result);
}

// Return a string in ascending order
const getSortedString = function(string) {return string.split('').sort().join('');}

```


### p2-random.js
```
/*
    CIT 281 Project 2
    Name: Brianna Wei
*/

// Returns a random number between min (inclusive) and max (exclusive)
function getRandomInteger(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

// Canvas posted solution for project 1
const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
let result = "";

for (let i = 0; i < getRandomInteger(5, 26); i++) {
    result += alphabet[getRandomInteger(1,alphabet.length-1)];
}

console.log(getRandomString(10,20));

// return a single, random, lowercase letter
function getRandomLetter() {
    const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
    let randomLetter = getRandomInteger(0,25);
    return alphabet[randomLetter];
}

// return the random length string
function getRandomString(minLength,maxLength) {
    let result = "";
    const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
    let randomChar = getRandomInteger(minLength,maxLength);
    for (let i=0; i < randomChar; i++) {
        result = result + getRandomLetter();
    }
    console.log(result);
}

// return a string in ascending order
function getSortedString(string) {
    return string.split('').sort().join('');
}

/*
// Code made for project 1, made by Brianna Wei

let letters = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z"];
let line = ""; 
let randomChar = getRandomInteger(5,25);
for (let i = 0; i < randomChar; i ++) {
    let randomIndex = getRandomInteger(0,25);
    line = line + letters[randomIndex];
}

console.log(line);

*/

```
