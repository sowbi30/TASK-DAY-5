FOR THE GIVEN JSON ITERATE OVER ALLFOR LOOPS (FOR, FORIN, FOR OF , FOR EACH)

Using a for...in loop (for iterating over object properties):

const jsonObject = {
  "name": "John",
  "age": 30,
  "city": "New York"
};

for (const key in jsonObject) {
  console.log(key, jsonObject[key]);
}
// ot name John
age 30
city New York


Using a for...of loop (for iterating over iterable values, not applicable to objects directly):

const jsonObject = {
  "name": "John",
  "age": 30,
  "city": "New York"
};

// Convert object values into an iterable array
const values = Object.values(jsonObject);

for (const value of values) {
  console.log(value);
}

// ot 
John
30
New York

Using a forEach loop (for iterating over object properties):

const jsonObject = {
  "name": "John",
  "age": 30,
  "city": "New York"
};

Object.keys(jsonObject).forEach(key => {
  console.log(key, jsonObject[key]);
});
//ot 
name John
age 30
city New York