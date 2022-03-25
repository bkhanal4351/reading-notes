# Functional Programming Concepts

. What is functional programming?
- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

. What is a pure function and how do we know if something is a pure function?
  - It returns the same result if given the same arguments (it is also referred as deterministic)
  - It does not cause any observable side effects

. What are the benefits of a pure function?
- The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts.

. What is immutability?
- When data is immutable, its state cannot change after it’s created.

. What is Referential transparency?
- if a function consistently yields the same result for the same input, it is referentially transparent.


# Node JS Tutorial for Beginners #6 - Modules and require()

. What is a module?
- Module in Node. js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node. js application. Each module in Node. js has its own context, so it cannot interfere with other modules or pollute global scope.

. What does the word ‘require’ do?
- The require() method is used to load and cache JavaScript modules.

. How do we bring another module into the file the we are working in?
- By using require keyword at the top of the file.

. What do we have to do to make a module available?
- By exporting modules.

notes taken from (https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)



