# JavaScript Core Lab 4

## Project Description

This project was created for Laboratory Work #4.
The main topics are JavaScript functions, closures, classes, inheritance, and unit testing.

## Project Structure

```text
js-core-sapar/
├── src/
│   ├── functions.js
│   └── Store.js
├── tests/
│   ├── functions.test.js
│   └── Store.test.js
├── package.json
├── README.md
└── .gitignore
```

## Implemented Functions

The project contains the following functions:

* `unique(arr)` — removes duplicate values from an array.
* `groupBy(arr, keyFn)` — groups objects by a calculated key.
* `chunk(arr, size)` — splits an array into smaller parts.
* `deepClone(obj)` — creates a deep copy of an object without using JSON serialization.
* `memoize(fn)` — saves previous function results using a closure.
* `counter()` — creates a counter using a closure.

Higher-order functions such as `map`, `filter`, and `reduce` are used in the project. Destructuring and spread syntax are also used.

## Store Class

The `Store` class contains:

* private field `#items`;
* `add()` method;
* `remove()` method;
* `find()` method;
* `total()` method;
* `items` getter;
* static `from()` method.

The `SortedStore` class inherits from `Store` and overrides methods using `super`.

## How to Run Tests

Install dependencies:

```bash
npm install
```

Run tests:

```bash
npm test
```

## Closures in My Code

A closure allows a function to remember variables from its outer scope.
I used closures in the `counter()` function to store the current counter value.
The returned functions can change and read this value even after the outer function has finished.
I also used a closure in `memoize()` to store previous function results.
The cache remains available between function calls.
This helps avoid repeating the same calculations.

## Test Results

The project contains unit tests for the implemented functions and classes.

Current test result:

```text
Test Files: 2 passed
Tests: 22 passed
```

### Passing Tests Screenshot

![Passing tests](tests-passing.png)

## AI Tools Used

ChatGPT was used to assist with code structure, explanations, debugging, and preparation of the laboratory work.
