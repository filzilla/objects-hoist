## Scope, hoisting and compartmentalization

### Answer the following:
In you own words, explain the concepts of scope, hoisting, compartmentalization.

There are two kinds of scope.  A global scope is when a variable is defined outside of
a function.  Local scope is when a variable is defined within a function, thus restricting
its use to with that function only.

Hoisting is the way javascript loads and uses functions and variables.  Javascript will read the code, then
will re-order the code.  It will put all functions and variable declarations at the top.
This way, the code can use the code from variables or functions that have been written later in the code.
As a rule, its a better practice to declare variables at the top of your code, to avoid hoisting problems.

Compartmentalization is breaking large code into bite size pieces. This helps to make it more re-usable,
and more the variables being used more secure.
### Provide examples for all three, below:

#### Scope:
 global variable example:

 var car = "Cadillac";

local variable example:

 function Car(){
   var car = "Toyota";
 }
#### Hoisting:

x = 1
function(){
  console.log(x);
};
var x;

JS will move to var x to the top of the code, even though
it was declared last, this way it can be used by the code.

#### Compartmentalization:

if we needed to write some code to do some math, we
could compartmentalize like this:

function doTheMath(); returns a value a.

function useTheMath(); takes the value from a and uses it.

function doTheMath(); returns a value b.

By organizing it like this, it can be re-used.
