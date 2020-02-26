# Eloquent JavaScript
- unary operators (- to negate a number, ! to negate logically, and typeof to find a value’s type) and a ternary operator (?:) to pick one of two values based on a third value.
- In pre-2015 JavaScript, only functions created new scopes, so old-style bindings, created with the var keyword, are visible throughout the whole function that they appear in—or throughout the global scope, if they are not in a function. let x = 10; if (true) {   let y = 20;   var z = 30;   console.log(x + y + z);   // → 60 } // y is not visible here console.log(x + z); // → 40
- There’s an Object.assign function that copies all properties from one object into another. let objectA = {a: 1, b: 2}; Object.assign(objectA, {b: 3, c: 4}); console.log(objectA); // → {a: 1, b: 3, c: 4} Arrays, then, are just a kind of object specialized for storing sequences of things.
- Values of type string, number, and Boolean are not objects, and though the language doesn’t complain if you try to set new properties on them, it doesn’t actually store those properties. As mentioned earlier, such values are immutable and cannot be changed.
- The more names have been taken, the more likely you are to accidentally overwrite the value of some existing binding.
- awkward to read is that we have a binding pointing at our array,
