# Read 2


## 1. Why would you want to run JavaScript code outside of a browser?
  - because javascript is a runtime environment which willmake it fasterand gie it a good ability to being used in different feilds.
  

## 2. What is the difference between a module and a package?
  - The module is where the package is being modified in details.
  - The package is a snip of code that can be used by another person.

## 3. What does the node package manager do?
  - It install the packages from the npm library and moderate all proceses related to the packages such as adding puckage by your own.

## 4. Provide code snippets showing 3 different ways to export a function from a node module

* `const getName = () => {
  return 'Jim';
};

const getLocation = () => {
  return 'Munich';
};

const dateOfBirth = '12.01.1982';

exports.getName = getName;
exports.getLocation = getLocation;
exports.dob = dateOfBirth;

// index.js 
const user = require('./user');
console.log(
  `${user.getName()} lives in ${user.getLocation()} and was born on ${user.dob}.`
);

`

* `
//file callsed user 
exports.getName = () => {
  return 'Jim';
};

exports.getLocation = () => {
  return 'Munich';
};

exports.dob = '12.01.1982';

// use the file
const { getName, dob } = require('./user');
console.log(
  `${getName()} was born on ${dob}.`
);
`

* `
class User {
  constructor(name, age, email) {
    this.name = name;
    this.age = age;
    this.email = email;
  }

  getUserStats() {
    return '
      Name: ${this.name}
      Age: ${this.age}
      Email: ${this.email}
    ';
  }
}

module.exports = User;

// in index.js
const User = require('./user');
const jim = new User('Jim', 37, 'jim@example.com');

console.log(jim.getUserStats());

`



