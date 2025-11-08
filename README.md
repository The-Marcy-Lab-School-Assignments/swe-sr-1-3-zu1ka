# swe-sr-1-3

## Setup

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/how-tos/working-with-assignments#how-to-work-on-assignments).

Here are some useful commands to remember.

```sh
npm i                   # install dependencies
git checkout -b draft   # switch to the draft branch before starting

git add -A              # add a changed file to the staging area
git commit -m 'message' # create a commit with the changes
git push                # push the new commit to the remote repo
```
## Question 1

Read the documentation for `findIndex` and `indexOf` on MDN:
- [findIndex](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex)
- [indexOf](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf). 

Explain the difference between the methods and explain when you would choose one over the other. Provide examples to enhance your response.

### Response

indexOf and findIndex are both methods used to find the position of an element in an array, but they work differently. IndexOf()  searches for an exact value in an array and returns its index. If the value is not found, it returns -1. It works best for simple values like numbers or strings. For example:

```javascript
const fruits = ['apple', 'banana', 'cherry'];
console.log(fruits.indexOf('banana')); 
console.log(fruits.indexOf('orange'));

```


findIndex is more flexible because it uses a callback function to test each element. It returns the index of the first element that meets a condition. If the condition isn’t met, it returns -1. This is useful when working with objects or complex conditions.For example:
```javascript
const users = [
  { name: 'zulka', age: 23 },
  { name: 'Bob', age: 30 },
  { name: 'Charlie', age: 35 }
];

const index = users.findIndex(user => user.age < 30);
console.log(index);

```
### When to Choose
- Use indexOf for simple value searches.
- Use findIndex when you need more complex conditions, like searching objects or ranges.




