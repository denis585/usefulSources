<p>
function multiplier(factor) { 
  return number => number * factor; }

let twice = multiplier(2); 
console.log(twice(5)); 
// → 10
</p>
The explicit local binding from the wrapValue example isn't really needed since a parameter is itself a local binding. Thinking about programs like this takes some practice. A good mental model is to think of function values as containing both the code in their body and the environment in which they are created. When called, the function body sees the environment in which it was created, not the environment in which it is called.
