Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

## Getting To Know Array Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (2-3 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your words what this method does.
6. Does it mutate the original value or not (check https://doesitmutate.xyz)

Example:

1. `concat`

   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.concat(4); //[1,2,3,4]
     let sentanceArray = "A quick brown fox jumped over a lazy".split(" ");
     sentanceArray.concat("dog").join(" "); //"A quick brown fox jumped over a lazy dog"
     let colors = ["red", "green", "blue"];
     colors.concat("black", "red", 21, true); // ['red','green','blue','black', 'red', 21, true]
     ```
   - `concat` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

2. `join`

- Parameter: separator (Optional) Specifies a string to separate each pair of adjacent elements of the array. The separator is converted to a string if necessary. If omitted, the array elements are separated with a comma (","). If separator is an empty string, all elements are joined without any characters in between them.
  - Return: A string with all array elements joined. If arr.length is 0, the empty string is returned.
  - Example:
    ```js
    var a = ["Wind", "Water", "Fire"];
    console.log(a.join()); //'Wind,Water,Fire'
    a.join(" + "); // 'Wind + Water + Fire'
    ```
  - No it does not mutate the original array.

3. `flat`

- Parameter: The flat() method creates a new array with all sub-array elements concatenated into it recursively up to the specified depth. depth (Optional). The depth level specifying how deep a nested array structure should be flattened. Defaults to 1.
  - Return: A new array with the sub-array elements concatenated into it.
  - Example:
    ```js
    const arr1 = [0, 1, 2, [3, 4]];
    console.log(arr1.flat()); // expected output: [0, 1, 2, 3, 4]
    const arr2 = [0, 1, 2, [[[3, 4]]]];
    console.log(arr2.flat(2)); // expected output: [0, 1, 2, [3, 4]]
    ```
  - It does mutate the original array.

4. `push`

- Parameter: The push() method adds one or more elements to the end of an array and returns the new length of the array.
  - Return:The new length property of the object upon which the method was called.
  - Example:
    ```js
    const animals = ["pigs", "goats", "sheep"];
    const count = animals.push("cows");
    console.log(count); // expected output: 4
    ```
  - It does mutate the original array.

5. `indexOf`

- Parameter: The indexOf() method returns the first index at which a given element can be found in the array, or -1 if it is not present. searchElement, Element to locate in the array. fromIndex (Optional) The index to start the search at. If the index is greater than or equal to the array's length, -1 is returned, which means the array will not be searched. If the provided index value is a negative number, it is taken as the offset from the end of the array. Note: if the provided index is negative, the array is still searched from front to back. If the provided index is 0, then the whole array will be searched. Default: 0 (entire array is searched).
  - Return:The first index of the element in the array; -1 if not found.
  - Example:
    ```js
    const beasts = ["ant", "bison", "camel", "duck", "bison"];
    console.log(beasts.indexOf("bison")); // expected output: 1
    ```
  - It does not mutate the original array.

6. `lastIndexOf`

- Parameter: The lastIndexOf() method returns the last index at which a given element can be found in the array, or -1 if it is not present. The array is searched backwards, starting at fromIndex.
  - Return:The first index of the element in the array; -1 if not found.
  - Example:
    ```js
    const animals = ["Dodo", "Tiger", "Penguin", "Dodo"];
    console.log(animals.lastIndexOf("Dodo")); // expected output: 3
    ```
  - It does not mutate the original array.

7. `includes`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

8. `reverse`

- Parameter:The reverse() method reverses an array in place. The first array element becomes the last, and the last array element becomes the first.

  - Return: The reversed array.
  - Example:

    ```js
    const a = [1, 2, 3];

    console.log(a); // [1, 2, 3]

    a.reverse();

    console.log(a); // [3, 2, 1]
    ```

  - It does mutate the original array.

9. `every`

- Parameter:The every() method tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value.

  - Return:true if the callbackFn function returns a truthy value for every array element. Otherwise, false.
  - Example:

    ```js
    const isBelowThreshold = (currentValue) => currentValue < 40;

    const array1 = [1, 30, 39, 29, 10, 13];

    console.log(array1.every(isBelowThreshold)); // expected output: true
    ```

  - It does not mutate the original array.

10. `shift`

- Parameter:The shift() method removes the first element from an array and returns that removed element. This method changes the length of the array.

  - Return:The removed element from the array; undefined if the array is empty.
  - Example:
    ```js
    const array1 = [1, 2, 3];
    const firstElement = array1.shift();
    console.log(array1); // expected output: Array [2, 3]
    console.log(firstElement); // expected output: 1
    ```
  - It does mutate the original array.

11. `splice`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

12. `find`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

13. `unshift`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

14. `findIndex`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

15. `filter`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

16. `flat`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

17. `forEach`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

18. `map`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

19. `pop`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

20. `reduce`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

21. `slice`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.

22. `some`

- Parameter:The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
  - Return:A boolean value which is true if the value searchElement is found within the array (or the part of the array indicated by the index fromIndex, if specified).
  - Example:
    ```js
    const array1 = [1, 2, 3];
    console.log(array1.includes(2)); // expected output: true
    ```
  - It does not mutate the original array.
