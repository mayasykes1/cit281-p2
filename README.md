[p2-random-commits.txt](https://github.com/user-attachments/files/15780150/p2-random-commits.txt)# CIT281 Project 2

### Learning Objectives:
<li>Gain experience using git via your CLI and Visual Studio Code (VSCode) Source Control</li>
<li>Gain experience writing and executing non-web server Node.js JavaScript code</li>
<li>Practice refactoring JavaScript code</li>

### Project Elements:
<li>Use the command line interface (CLI) of your operating system to create and work with a git repository (repo)</li>
<li>Refactor the JavaScript program from the previous project to practice using git and practice refactoring</li>
<li>Use git via VSCode (Create and use a .gitignore file / diff split screen)</li>

### Code:

#### p2-expressions.js
<code>getRandomInteger = (min, max) => {
    return Math.floor(Math.random() * (max - min) + min);
  } 
  getRandomLetter = () => {
    const alphabet = "abcdefghijklmnopqrstuvwxyz";
    return alphabet[getRandomInteger(0, alphabet.length)];
  }
  getRandomString = (minLength, maxLength) => {
    let result = "";
    for (let i = 0; i < getRandomInteger(minLength,maxLength + 1); i++) {
    result += getRandomLetter();
  }
    return result;
  }
  getSortedString = (string) => {
    return string.split("").sort().join(''); 
  }
  console.log(getSortedString("xpacd"));</code>

#### p2-random.js
<code>function getRandomInteger(min, max) {
  return Math.floor(Math.random() * (max - min) + min);
}
function getRandomLetter() {
  const alphabet = "abcdefghijklmnopqrstuvwxyz";
  return alphabet[getRandomInteger(0, alphabet.length)];
}
function getRandomString(minLength, maxLength) {
  let result = "";
  for (let i = 0; i < getRandomInteger(minLength,maxLength + 1); i++) {
  result += getRandomLetter();
}
  return result;
}
function getSortedString(string) {
  return string.split("").sort().join(''); 
}
console.log(getSortedString("xpacd"));</code>
  
### Photos:
<img width="1237" alt="p2-vscode-diff" src="https://github.com/mayasykes1/cit281-p2/assets/52678410/5ac0bd08-f747-4ac5-9109-c97b2ee16f95">
