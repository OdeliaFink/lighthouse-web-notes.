let myGlobalVar = "global";

const printMyVars = function() {
  let myLocalVar = "local";
  console.log("-- Inside printMyVars --");
  console.log("myLocalVar is:", myLocalVar);
  console.log("myGlobalVar is:", myGlobalVar);
}

printMyVars();

console.log('-- Outside of printMyVars now --');
console.log(myLocalVar);

Double Equals, Triple Equals, and Type Coercion:

Type Coercion: When the operands of an operator are different types, one of them will be converted to an equivalent value of the other operand's type

The === does not only compare two values, but also the type of those values.
the == operator will attempt to force the two values to be of the same type, if possible. This is called type coercion, and it can really mess up your expected results if you're not careful.

Falsey:
False
0
""
null
undefined
NaN