# JS Functions Week1 Homework2

## Instructions
1. Fork and clone this repository.
2. Change into the new directory`cd w01d03-HW2`
3. Create a file called solution.js and add all answers to it. 
---

#### Exercise 1:
Research 3 string methods and describe what they are used for and how to use them.  You can find string methods here https://www.w3schools.com/js/js_string_methods.asp

Method 1
```
Name: String Length
Description: The length property returns the length of a string.

Example using it: 
var txt = "Mohammed Alghamdi";
var sln = txt.length;
```

Method 2
```
Name: Finding a String in a String
Description: The indexOf() method returns the index of (the position of) the first occurrence of a specified text in a string.
Example using it:
var str = "Hellow, Welcome to GA";
var pos = str.indexOf("GA");
```

Method 3
```
Name: Searching for a String in a String
Description: The search() method searches a string for a specified value and returns the position of the match:
Example using it:
var str = "Please locate where 'locate' occurs!";
var pos = str.search("locate");

```
---

#### Exercise 2:
Where can you print out the value of variable c without resulting in an error?

```js
var a = 1;
function x() {
  var b = 2;
  function y() {
    var c = 3;
    function z() {
      var d = 4;
    }
    z();
  }
  y();
}

x();
```
1. anywhere in the script! 
2. anywhere inside the function `x()` 
3. anywhere inside the function `y()`   ***
4. anywhere inside the function `z()`

Answer is:  anywhere inside the function `y()`

### Choose the correct answer

---

#### Exercise 3: Dice Roller
- Write a function that chooses two random numbers (1-6) and returns them. It should also return the sum.
- Example: `rollDice() // Dice rolled are 6 and 1.  Sum is 7`
- BONUS: have your function take an argument of the # of dice to be rolled.
- Example: `rollDice(3) // Dice rolled are 4, 2, and 7.  Sum is 13.`

Answer:

function x (){
  var num1 = Math.floor(Math.random()*6)+1;
  var num2 = Math.floor(Math.random()*6)+1;
  var result = num1 + num2;
  return "Dice rolled are " + num1 + " and " + num2 + ". Sum is " + result;
}


console.log(x());


---

#### Exercise 4: currencyConverter(currency, amount)
  - Write a function `currencyConverter` that takes two arguments an amount and a currency (USD, GBP, EGP, BD) and returns  the converted version of the amount in Riyals. 
  - Use the if-then-else construct available in Javascript.
**Hint :**
> - 1 Riyal = 4.68 Egyptian pound 
> - 1 Riyal = 0.10 Bahraini dinar


Answer:

function currencyConverter (amount,currency){
  if (currency == "USD"){
    let convertedVersion = amount * 0.266667;
    return convertedVersion;
  }else if (currency == "EGP"){
    let convertedVersion = amount * 4.29319;
    return convertedVersion;
  }else if (currency == "GBP"){
    let convertedVersion = amount * 0.206290;
    return convertedVersion;
  }else if (currency == "BD"){
    let convertedVersion = amount * 0.100267;
    return convertedVersion;
  }
}
---

### BONUS 5,6
#### Exercise 5: isCharacterAVowel(character)
  - Write a function `isCharacterAVowel` that takes a character (i.e. a string of length 1) and returns true if it is a vowel and false, otherwise.
---
#### Exercise 6: pow(base, exponent)
  - Define a function `pow` that replicates the [Math.pow()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/pow) method in JavaScript's Math object.

---
### Deliverable  
1. When finished, `git add .`, `git commit -m " "`, `git push origin master` to your fork and submit a pull request.
2. Please fill up the following questions when you pull request:
- on a scale from 1 to 5, how comfortable were you with this assignment? (1 is very difficult)
- How long did it take?
- What was a challenge you had with this assignment?
- Is there anything that you'd like some further information on?
- Do you have any suggestions to improve this assignment?
