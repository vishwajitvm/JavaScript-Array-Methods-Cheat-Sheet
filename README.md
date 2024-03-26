# JavaScript Array Methods Cheat Sheet - Fruits Edition

This cheat sheet provides a quick reference for JavaScript array methods, using examples involving fruits.

Credits: Axel Rauschmayer

## Adding or removing an element at either end of an Array:

| Array Before       | Method                | Return Value | Array After           | Definition                                   | Example |
|--------------------|-----------------------|--------------|-----------------------|------------|---------|
| ["Apple","Banana"] | .push("Orange")       | 3            | ["Apple","Banana","Orange"] | Adds one or more elements to the end of an array and returns the new length of the array. | `fruits.push("Orange")` adds "Orange" to the end of the array. |
| ["Apple","Banana"] | .pop()                | "Banana"     | ["Apple"]             | Removes the last element from an array and returns that element. | `var removed = fruits.pop()` removes "Banana" from the end of the array. |
| ["Apple","Banana"] | .unshift("Orange")    | 3            | ["Orange","Apple","Banana"] | Adds one or more elements to the beginning of an array and returns the new length of the array. | `fruits.unshift("Orange")` adds "Orange" to the beginning of the array. |
| ["Apple","Banana"] | .shift()              | "Apple"      | ["Banana"]            | Removes the first element from an array and returns that removed element. | `var removed = fruits.shift()` removes "Apple" from the beginning of the array. |
|                    |                       |              |                       | | |
| ["Apple","Banana"] | .unshift(arr.pop())   | 2            | ["Banana","Apple"]    | Removes the last element from one array and adds it to the beginning of another array. | `fruits.unshift(arr.pop())` removes "Banana" from `arr` and adds it to the beginning of `fruits`. |

## Changing all of an Array (the input Array is modified and returned):

| Array Before             | Method                      | Return Value                        | Definition | Example |
|--------------------------|-----------------------------|-------------------------------------|------------|---------|
| ["Apple","Banana","Orange"] | .fill("Pear")             | ["Pear","Pear","Pear"]              | Fills all the elements of an array with a static value. | `fruits.fill("Pear")` fills the array with "Pear". |
| Array(4)                | .fill("Kiwi")               | ["Kiwi","Kiwi","Kiwi","Kiwi"]       | Fills all the elements of a typed array with a static value. | `typedArray.fill("Kiwi")` fills the typed array with "Kiwi". |
| Array(4)                | .fill("Kiwi").map( (val,idx) => idx ) | [0, 1, 2, 3]                | Fills all the elements of an array with a static value and then maps each element to its index. | `fruits.fill("Kiwi").map((val,idx) => idx)` fills the array with "Kiwi" and then maps each element to its index. |
| ["Apple","Banana","Orange"] | .reverse()                | ["Orange","Banana","Apple"]         | Reverses the order of the elements in an array. | `fruits.reverse()` reverses the array order. |
| ["Cherry","Apple","Durian","Banana"] | .sort()             | ["Apple","Banana","Cherry","Durian"]| Sorts the elements of an array in place and returns the sorted array. | `fruits.sort()` sorts the array alphabetically. |
| ["Apple","Banana","Orange"] | .sort()                   | ["Apple","Banana","Orange"]         | Sorts the elements of an array in place and returns the sorted array. | `fruits.sort()` sorts the array alphabetically. |
| ["Apple","Banana","Orange"] | .copyWithin(1,2,3)        | ["Apple","Orange","Orange","Orange"]| Copies a sequence of elements within the array to the position starting at target. | `fruits.copyWithin(1,2,3)` copies "Orange" to the index starting at 1.|

## Finding Array elements:

| Array                    | Method                  | Return Value | Definition | Example |
|--------------------------|-------------------------|--------------|------------|---------|
| ["Apple","Banana","Orange"] | .includes("Banana")   | true         | Determines whether an array includes a certain value among its entries. | `fruits.includes("Banana")` returns true. |
| ["Apple","Banana","Orange"] | .indexOf("Banana")    | 1            | Returns the first index at which a given element can be found in the array, or -1 if it is not present. | `fruits.indexOf("Banana")` returns 1. |
| ["Apple","Banana","Apple"]  | .lastIndexOf("Apple") | 2            | Returns the last index at which a given element can be found in the array, or -1 if it is not present. | `fruits.lastIndexOf("Apple")` returns 2. |
| ["Apple","Banana","Orange"] | .find(x => x === "Banana") | "Banana" | Returns the first element in the array that satisfies the provided testing function. | `fruits.find(x => x === "Banana")` returns "Banana". |
| ["Apple","Banana","Orange"] | .findIndex(x => x === "Banana") | 1 | Returns the index of the first element in the array that satisfies the provided testing function. | `fruits.findIndex(x => x === "Banana")` returns 1. |

## Creating a new Array from an existing Array:

| Array Before       | Method (links to MDN)    | Return Value        | Definition | Example |
|--------------------|--------------------------|---------------------|------------|---------|
| ["Apple","Banana","Orange"] | .slice(1, 2)        | ["Banana","Orange"] | Extracts a section of an array and returns a new array. | `var newFruits = fruits.slice(1, 2)` returns ["Banana","Orange"]. |
| ["Apple","Banana","Orange"] | .splice(1, 2)       | ["Banana","Orange"] | Changes the contents of an array by removing or replacing existing elements and/or adding new elements in place. | `var removed = fruits.splice(1, 2)` removes "Banana" and "Orange" from the array. |
| ["Apple","Banana","Apple"]  | .filter(x => x === "Apple") | ["Apple","Apple"] | Creates a new array with all elements that pass the test implemented by the provided function. | `var apples = fruits.filter(x => x === "Apple")` returns ["Apple","Apple"]. |
| ["Apple","Banana"]  | .map(x => x+x )       | ["AppleApple", "Ban





# JavaScript Array Methods Cheat Sheet - Fruits Edition

This repository contains a cheat sheet for JavaScript array methods, using examples involving fruits. It serves as a quick reference for developers when working with arrays in JavaScript.

## Original Credit

This cheat sheet is based on the work of Axel Rauschmayer.

## Original Cheat Sheet

The original cheat sheet with examples involving shapes and colors can be found [here](https://array-methods.github.io/).

## Usage

Feel free to refer to this cheat sheet whenever you need a quick reminder of how different array methods work in JavaScript.

## Contribution

Contributions are welcome! If you have any improvements or additional examples to add, please feel free to submit a pull request.

## Credits

- Axel Rauschmayer for the original cheat sheet.

## License

This cheat sheet is open source under the [MIT License](LICENSE).

