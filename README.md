# hello
###
(https://www.codewars.com/kata/find-the-calculation-type/train/javascript)
You have to create a function which receives 3 arguments: 2 numbers, and the result of an unknown operation performed on them (also a number).

Based on those 3 values you have to return a string, that describes which operation was used to get the given result.

The possible return strings are: "addition", "subtraction", "multiplication", "division".

```javascript
function calcType(a, b, res) {
  if( a + b === res){
  return 'addition';
  }
  if( a - b === res){
  return 'subtraction';
  }
  if( a * b === res){
  return 'multiplication';
  }
  if( a / b === res){
  return 'division';
  }
}
```
###

(https://www.codewars.com/kata/simple-beads-count/train/javascript)
 ###
 #Task
 
 Two red beads are placed between every two blue beads. There are N blue beads. After looking at the arrangement below work out the number of red beads.
 
 @ @@ @ @@ @ @@ @ @@ @ @@ @
 
 Implement count_red_beads(n) (in PHP count_red_beads($n); in Java, Javascript, TypeScript, C, C++ countRedBeads(n)) so that it returns the number of red beads.
 If there are less than 2 blue beads return 0.
 
 ###
 Solution
 ```javaskript
 function countRedBeads(n) {
  
    if (n < 2) {
    return 0;
 }
 return (n - 1) * 2;
 }
 ```
 
 (https://www.codewars.com/kata/reverse-a-number/train/javascript)
 
 #Task
 ###
 Given a number, write a function to output its reverse digits. (e.g. given 123 the answer is 321)
 
 Numbers should preserve their sign; i.e. a negative number should still be negative when reversed.
 ###
 Solution
 ```javaskript
 function reverseNumber(n) {
 if (n >= 0){
   let arr = n.toString().split('').reverse();
   return +(arr.join(''));
   }else {
   n = n * (-1);
   let arr = n.toString().split('').reverse();
   return (-1) * (+(arr.join('')));
   }
 }
 ```
 ###
 (https://www.codewars.com/kata/numerical-palindrome-number-1/train/javascript)
 #Task
 ###
 
 A palindrome is a word, phrase, number, or other sequence of characters which reads the same backward as forward. Examples of numerical palindromes are:
 
 2332 
 110011 
 54322345
 
 For a given number num, write a function to test if it's a numerical palindrome or not and return a boolean (true if it is and false if not). Return "Not valid" if the input is not an integer or less than 0.
 ###
 Solution
 ```javaskript
 function palindrome(num) { 
  let str = "";
    if (typeof num !== 'number' || num < 0){
    return  'Not valid';
    }
    str = num + '';
  
   for (let i = 0; i < Math.floor(str.length / 2); i++){
   if (str[i] !== str[str.length -i -1]) {
   return false;
   }
   }
   ```
 
 
 
 
