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
 ###
 (https://www.codewars.com/kata/53da6d8d112bd1a0dc00008b)
 ###
 #Task
 In this kata you will create a function that takes in a list and returns a list with the reverse order.
 
 Examples
 reverseList([1,2,3,4]) == [4,3,2,1]
 reverseList([3,1,5,4]) == [4,5,1,3]
 ###
 Solution
 ```Javaskript
 function reverseList(list) {
 let arr = [];
 for (let i = list.length -1; i >= 0; i--){
   arr.push(list[i]);
  }
  return arr
 }
 ```
 ###
 (https://www.codewars.com/kata/students-final-grade/train/javascript)
 ###
 #Task
 This function should take two arguments: exam - grade for exam (from 0 to 100); projects - number of completed projects (from 0 and above);
 
 This function should return a number (final grade). There are four types of final grades:
 
 100, if a grade for the exam is more than 90 or if a number of completed projects more than 10.
 90, if a grade for the exam is more than 75 and if a number of completed projects is minimum 5.
 75, if a grade for the exam is more than 50 and if a number of completed projects is minimum 2.
 0, in other cases
 Examples:
 
 finalGrade(100, 12);  // 100
 finalGrade(99, 0);    // 100
 finalGrade(10, 15);   // 100
 
 finalGrade(85, 5);    // 90
 
 finalGrade(55, 3);    // 75
 
 finalGrade(55, 0);    // 0
 finalGrade(20, 2);    // 0
 #
 Solution
 ```Javaskript
 function finalGrade (exam, projects) {
   if (exam > 90 || projects > 10) return 100;
   if (exam > 75 && projects >= 5) return 90;
   if (exam > 50 && projects >= 2) return 75;
   if (exam > 90 || projects > 10) return 100;
     return 0;
 }
 ```
 ###
 (https://www.codewars.com/kata/remove-string-spaces/train/javascript)
 ###
 #Task
 Simple, remove the spaces from the string, then return the resultant string.
 #
 Solution
 ```Javaskript
 function noSpace(x){
 let str = x.replace (/ /g, '');
 return str;
 }
 ```
 
 ###
 (https://www.codewars.com/kata/switch-it-up/train/javascript)
 #
 Task
 When provided with a number between 0-9, return it in words.
 
 Input :: 1
 
 Output :: "One".
 
 Try using "Switch" statements.
 ###
 Solution1
 ```Javaskript
 function switchItUp(number){
 let arr = ['Zero', 'One', 'Two', 'Three', 'Four', 'Five', 'Six', 'Seven', 'Eight', 'Nine',];
 return arr[number];
 }
 ```
 
 