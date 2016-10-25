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
  
