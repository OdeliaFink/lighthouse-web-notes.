Callbacks:

const myFn = function() {
  console.log("I am function.");
}

myFn.someAttribute = 42
console.log(myFn.someAttribute);

function runner(f) {
  f()
}

runner(myFn);

1) Assigning a function to myFn variable 
2) someAttribute assigned to myFn object
3) A runner function runs argument f and is passed
4) Pass reference myFn and is evoked by runner function 

----------------------------

-- Callback is a function passed (by reference) into another function (let's call that one the "receiver" function)
-- The receiver function is therefore accepting behavior to perform by calling the callback function that it now has access to
-- The receiver function can decide to call the callback function at any time, as many times as it wants

Another example:

const findWaldo = function(names, found) {
  for (let i = 0; i < names.length; i++) {
    let name = names[i];
    if (name === "Waldo") {
      found();   // execute callback
    }
  }
}

const actionWhenFound = function() {
  console.log("Found him!");
}

findWaldo(["Alice", "Bob", "Waldo", "Winston"], actionWhenFound);