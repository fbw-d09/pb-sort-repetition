## sort()

:large_blue_circle:The `sort()` method sorts the elements of an array and returns the reference to the same array, now sorted. The default sort order is ascending, built upon converting the elements into strings, then comparing their sequences of UTF-16 code units values.

---
`console.log()` both arrays and have a look how they get sorted, when using `sort()` only by default.

```javascript
const stringArray = ["ba", "f", "ea", "cf", "baa", "b"];

const numberArray = [ 1, 20, 10, 250, -8, 43]

console.log(stringArray.sort());

console.log(numberArray.sort())
```
---
:large_blue_circle:`sort()` can take a function as an optional parameter, which helps us to define the sort order. `array.sort(compareFunction)`

```javascript
function compareFunction(a, b) {
  if (a is less than b by some ordering criterion) {
    return -1;
  }
  if (a is greater than b by the ordering criterion) {
    return 1;
  }
  // a must be equal to b
  return 0;
}
```

:large_blue_circle: you can also pass an arrow function directly `array.sort((a, b) => { /* … */ } )`

-----
## :cartwheeling: Exercise

1. The `charCodeAt()` method :point_right:[mdn charCodeAt()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charCodeAt) returns an integer between 0 and 65535 representing the UTF-16 code unit at the given index. Sort the letters array and print the code unit for each letter of the letters array. 


`const letters = ["a", "u", "t", "p", "x"]`

---

2. Create an array, which holds 6 firstnames of the Breaking Bugs and sort the array according to the length of the names. 
The sorted array should start with the shortest name.

```javascript
const fourZeroFiveFound = ["Melanie" , "Hansi", "Ruben", "Zoe", "Dirk", "Rick"]

after sort the array should look like that:

console.log(fourZeroFiveFound)

Output =>  [ 'Zoe', 'Dirk', 'Rick', 'Hansi', 'Ruben', 'Melanie' ]


```
---
3.1 Sort the number array in ascending order
```
const numberArray = [ 1, 20, 10, 250, -8, 43]
```
3.2 Sort the number array in descending order
```
const numberArray = [ 1, 20, 10, 250, -8, 43]
```
---
4. Sort the cart items according to the price

```javascript
const cart = [
    {article: "shoes", price: 49.99},
    {article: "laptop", price: 999.99},
    {article: "book", price: 29.49},
    {article: "coffee machine", price: 49.49},
]
```
---

    
