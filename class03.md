. What does .map() return?
- It returns an object of map class.

. If I want to loop through an array and display each value in JSX, how do I do that in React?
- By attaching map method to an array and pass a callback function that gets called for each iteration.

. Each list item needs a unique ____.
- Key

. What is the purpose of a key?
- Key is used to return an array of a given object.

. What is the spread operator?
- In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

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
- const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

. Give an example of using the spread operator to combine two objects into one.
- [...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
[..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }

notes taken from (https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)