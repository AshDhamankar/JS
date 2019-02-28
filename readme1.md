n number of arguments (variable parameter) - called rest arguments - define as (...arguments)...
arguments.length
arguments[i] where i is always a valid integer index into the arguments, and can not be out of bound
Never use arguments directly without .length or [i]

function manyArgs() {
  for (var i = 0; i < arguments.length; ++i)
    alert(arguments[i]);
}

With ECMAScript 6, you can use rest of arguments syntax:

const testArray = (...args) => {
    console.log(args);
}; testArray(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

=======
parametere vs arguments-
A parameter is a variable in a method definition.
When a method is called, the arguments are the data you pass into the method's parameters. 
Parameter is variable in the declaration of function. Argument is the actual value of this variable that gets passed to function.
=================
JS va TS - https://www.javatpoint.com/javascript-vs-typescript
=======
ES6 or typesctipt functionality

Javascript's ECMA6 came out with some cool new features; ... is one of these new Javascript functionalities. 
It can be used in two different ways; as a spread operator OR as a rest parameter.

Rest parameter: collects all remaining elements into an array.
Spread operator: allows iterables( arrays / objects / strings ) to be expanded into single arguments/elements.
