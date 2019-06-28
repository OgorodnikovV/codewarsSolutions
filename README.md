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
 ##Task
 Two red beads are placed between every two blue beads. There are N blue beads. After looking at the arrangement below work out the number of red beads.
 
 @ @@ @ @@ @ @@ @ @@ @ @@ @
 
 Implement count_red_beads(n) (in PHP count_red_beads($n); in Java, Javascript, TypeScript, C, C++ countRedBeads(n)) so that it returns the number of red beads.
 If there are less than 2 blue beads return 0.
 
 ###Solution
 ```javaskript
 function countRedBeads(n) {
  
    if (n < 2) {
    return 0;
 }
 return (n - 1) * 2;
 }
 ```
