Function to Filter Even Numbers:


function filterEvenNumbers(numbers) {
  return numbers.filter(num => num % 2 === 0);
}

// Example usage:
const numbersArray = [1, 2, 3, 4, 5, 6];
const evenNumbers = filterEvenNumbers(numbersArray);
console.log(evenNumbers); // Output: [2, 4, 6]

Function to Filter People Over 30:
function filterPeopleOver30(people) {
  return people.filter(person => person.age > 30);
}

// Example usage:
const peopleArray = [
  { name: 'John', age: 25, email: 'john@example.com' },
  { name: 'Jane', age: 35, email: 'jane@example.com' },
  { name: 'Bob', age: 28, email: 'bob@example.com' }
];
const peopleOver30 = filterPeopleOver30(peopleArray);
console.log(peopleOver30); // Output: [{ name: 'Jane', age: 35, email: 'jane@example.com' }]



Stack Data Structure using an Array:
class Stack {
  constructor() {
    this.items = [];
  }

  push(element) {
    this.items.push(element);
  }

  pop() {
    return this.items.pop();
  }

  peek() {
    return this.items[this.items.length - 1];
  }

  isEmpty() {
    return this.items.length === 0;
  }

  size() {
    return this.items.length;
  }
}

// Example usage:
const stack = new Stack();
stack.push(1);
stack.push(2);
console.log(stack.peek()); // Output: 2
console.log(stack.pop());  // Output: 2
console.log(stack.isEmpty()); // Output: false
Queue Data Structure using an Array:
javascript
Copy code
class Queue {
  constructor() {
    this.items = [];
  }

  enqueue(element) {
    this.items.push(element);
  }

  dequeue() {
    return this.items.shift();
  }

  front() {
    return this.items[0];
  }

  isEmpty() {
    return this.items.length === 0;
  }

  size() {
    return this.items.length;
  }
}

// Example usage:
const queue = new Queue();
queue.enqueue(1);
queue.enqueue(2);
console.log(queue.front()); // Output: 1
console.log(queue.dequeue());  // Output: 1
console.log(queue.isEmpty()); // Output: false
Function to Remove Vowels from a String:
javascript
Copy code
function removeVowels(inputString) {
  return inputString.replace(/[aeiouAEIOU]/g, '');
}

// Example usage:
const originalString = 'Hello, World!';
const stringWithoutVowels = removeVowels(originalString);
console.log(stringWithoutVowels); // Output: 'Hll, Wrld!'
Function to Return Unique Elements from Two Arrays:
javascript
Copy code
function uniqueElements(arr1, arr2) {
  const uniqueArr = [...new Set([...arr1, ...arr2])];
  return uniqueArr;
}

// Example usage:
const array1 = [1, 2, 3];
const array2 = [2, 3, 4, 5];
const resultArray = uniqueElements(array1, array2);
console.log(resultArray); // Output: [1, 2, 3, 4, 5]

