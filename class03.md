. What does .map() return?
- It returns an object of map class.

. If I want to loop through an array and display each value in JSX, how do I do that in React?
- By attaching map method to an array and pass a callback function that gets called for each iteration.

. Each list item needs a unique ____.
- Key

. What is the purpose of a key?
- Key is used to return an array of a given object.

. What is the spread operator?
- In JavaScript, spread syntax refers to the use of an ellipsis of three dots (âĶ) to expand an iterable object into the list of arguments.

. List 4 things that the spread operator can do.
  1. Copying an array
  2. Concatenating or combining arrays
  3. Using Math functions
  4. Using an array as arguments

. Give an example of using the spread operator to combine two arrays.

  -- Copying an array
  - const strArr = ['hello','world']
  const strArr2 = [...strArr]

  const spread = {...strArr,...strArr2}

. Give an example of using the spread operator to add a new item to an array.
- const fruits = ['ð','ð','ð','ð','ð']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "ð", "ð", "ð", "ð", "ð" ]
fruits[0] = 'ð'
console.log(...[...fruits,'...',...moreFruits]) //  ð ð ð ð ð ... ð ð ð ð ð

. Give an example of using the spread operator to combine two objects into one.
- [...["ððððĪŠð"]] // Array [ "ððððĪŠð" ]
[..."ððððððĨ°ððĪĐ!"] // Array(9) [ "ð", "ð", "ð", "ð", "ð", "ðĨ°", "ð", "ðĪĐ", "!" ]

const hello = {hello: "ððððĪŠð"}
const world = {world: "ððððððĨ°ððĪĐ!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "ððððĪŠð", world: "ððððððĨ°ððĪĐ!" }

notes taken from (https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)