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

'''script.js 
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
'''
