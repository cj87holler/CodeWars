# CodeWars
A compilation of CodeWars Challenges in JavaScript  

# Is this a triangle? 
Implement a method that accepst 3 integer values a, b, c. The method should return true if a triangle can be built with the sides of a given length and false in any other case. (In this case, all triangles must have surface greater than 0 to be accepted). 

```script.js 
function isTrianlge(a, b, c){ 
  let max = Math.max(a,b,c); 
  let sum = a + b + c; 
  return sum - max > max; 
  } 
  ``` 
 Additional solution I really liked: 
 ```script.js 
 function isTriangle(a. b.c){ 
  return a + b > c && a + c > b && c + b > a; 
  } 
  ``` 
  
# Square Every Digit  
Welcome. In this kata, you are asked to square every digit of a number.
For example, if we run 9119 through the function, 811181 will come out.
Note: The function accepts an integer and returns an integer. 

```script.js 
function squareDigits(num){
  var num1 = num.toString(); 
  var num2 = num1.split(""); 
  var result = ' ';
  for (var i = 0; i < num2.length; i++) { 
  result += Math.pow( num2[i], 2); 
  }; 
  var test = parseInt(result); 

return test;
}
``` 

Additional solution I really liked: 
```script.js 
function squareDigits(num){ 
var array = num.toString().split('').map(function(int) { 
  var i = parseInt(int); 
  return i * i; 
  }); 
  return parseInt(array.join("")); 
  }  
  ```



# A square of squares

You like building blocks. You especially like building blocks that are squares. And what you even like more, is to arrange them into a square of square building blocks!

However, sometimes, you can't arrange them into a square. Instead, you end up with an ordinary rectangle! Those blasted things! If you just had a way to know, whether you're currently working in vain… Wait! That's it! You just have to check if your number of building blocks is a perfect square.

Task

Given an integral number, determine if it's a square number:

In mathematics, a square number or perfect square is an integer that is the square of an integer; in other words, it is the product of some integer with itself.
The tests will always use some integral number, so don't worry about that in dynamic typed languages.

```script.js

var isSquare = function(n){ 
	var number = n; 
  return(Math.sqrt(number)) % 1 === 0; 
  } 
  ``` 
 Additional solution I really liked: 
 ```script.js 
 var isSquare = function(n){ 
 	if(Math.sqrt(n) % 1) == 0) 
	return true; 
	else 
	return false; 
	} 
	```
