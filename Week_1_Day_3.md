const mary = { name: "Mary Sue" };
mary["name"] = "Mary Jane";
mary["age"]  = 22;
mary // shows the resulting object with both properties

const person = {
  name: "Paul",
  address: {
    street: "310 W 95th",
    city: "New York",
    zipCode: 10027
  }
};

nest objects above so to access street, i'd have to do person.address.street to get the value in street. 

** object keys are strings***

Object.keys(): inspects an object's keys and returns an array of keys

var planetMoons = {
  mercury: 0,
  venus: 0,
  earth: 1,
  mars: 2,
  jupiter: 67,
  saturn: 62,
  uranus: 27,
  neptune: 14
};
for (var planet in planetMoons) {
  var numberOfMoons = planetMoons[planet];
  console.log("Planet: " + planet + ", # of Moons: "+ numberOfMoons);
}
We have the key available to us within the scope of the loop; in the above example it is the planet variable. Notice how we access the object using a variable, planetMoons[planet]. The variable planet iterates over each key ("mercury", "venus", ...) using the for-loop.

const donut = {
  dough: "chocolate",
  glazing: "raspberry",
  sprinkles: false,
  price: 199
}

const keyToFetch = "dough"
// Bracket or dot notation

// Dot notation - Drax
console.log(donut.dough)
console.log(donut.keyToFetch)

// Bracket
console.log(donut["dough"])
console.log(donut[keyToFetch])

// commits[0].commit.author.main.principal.name.first_name
// commits[0]["commit"]["author"]["main"]
const donutPricePlusTaxes = Math.round(donut.price * 1.14975) / 100

console.log(`My best donut as a ${donut.dough} dough and it's ${donutPricePlusTaxes}`)

// For..of, for..in, Object.keys()


// Define a donut object
const peopleDonut = {
  dough: "Plain",
  glazing: "Rose Pistachio",
  sprinkles: true,
  price: 9999
}

const keysOfDonut = Object.keys(peopleDonut)

for (const key of keysOfDonut) {
  const value = peopleDonut[key]
  console.log(value)
}

// List all the keys of the donut
// Iterate over the keys of the donut
// Extract value of our donut object at the position of the key
// Output to the console the value

for (let i = 0; i < keysOfDonut.length; i++) {
  const key = keysOfDonut[i]
}

peopleDonut["price"] = 1
console.log(peopleDonut)