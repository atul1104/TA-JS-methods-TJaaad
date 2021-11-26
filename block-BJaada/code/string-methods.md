Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

#### Getting To Know String Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (4-5 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your own words and one sentence explain what this method does.

Example:

1.  `charAt`

    - Parameter: (index) defaults to 0 - (number data type)
    - Return: character at specific index in the string (string data type)
    - Example:
      ```js
      let name = "Arya Stark";
      name.charAt(2); //"y"
      let sentance = "A quick brown fox jumped over a lazy dog";
      sentance(4); // "i"
      let houseName = "Starks";
      houseName.charAt(0); // "S"
      ```
    - `charAt` accepts a index (number data type) and return the character on that index in the string.

2.  `toUpperCase`

    - Parameter: It takes no parameters.
      -Return: returns the string datatype value with uppercase. It does not affect the vvalue of string itself.
      -Example:

    ```js
    let name = "arya stark";
    name.toUpperCase(); // 'ARYA STARK'
    let user = "22";
    user.toUpperCase(); // '22'
    ```

3.  `toLowerCase`

    - Parameter: It takes no parameters.
      -Return: returns the string datatype value with uppercase. It does not affect the vvalue of string itself.
      -Example:

    ```js
    let name = "ARYA STARK";
    name.toLowerCase(); // 'arya stark'
    console.log("ALPHABET".toLowerCase()); // 'alphabet'
    ```

4.  `trim`
    Parameter: It accepts no parameter.
    Return: It removes the white spaces in the string
    Example:
    ```js
    let helloUser = "   Hello User   ";
    helloUser.trim(); //"Hello User"
    var orig = "   foo  ";
    console.log(orig.trim()); // 'foo'
    ```
5.  `trimEnd`
    Parameter: It accepts no parameter.
    Return: removes whitespace from the end of a string and returns a string withous white space at end of string.
    Example:

    ```js
    let str = "   Hello  ";
    str.trimEnd(); //'   Hello';
    const greeting = "   Hello world!   ";
    console.log(greeting.trimEnd()); // "   Hello world!";
    ```

6.  `trimStart`
    Parameter: It accepts no parameter.
    Return: removes whitespace from the start of a string and returns a string withous white space at start of string.
    Example:

    ```js
    let str = "   Hello  ";
    str.trimEnd(); //'Hello   ';
    const greeting = "   Hello world!   ";
    console.log(greeting.trimEnd()); // "Hello world!   ";
    ```

7.  `concat`
    Parameter: It accepts one or more strings to concat and produce new string. If the arguments are not of the type string, they are converted to string values before concatenating.
    Return: It returns new concatenated string.
    Example:

    ```js
    const str1 = "Hello";
    const str2 = "World";
    str1.concat(", ", str2); //'Hello, World'
    let str4 = "Happy";
    let str5 = "Diwali";
    let str3 = "To you all";
    str4.concat(" ", str5, " ", str3);
    ```

8.  `endsWith`
    Parameter: It accepts two parameters first is searchString(the character or letter we want to end with). also accepts length parameter(optional). By default it is set to the str.length. endsWith checks if the string is ended with the character specified in the steingSearch as a parameter.
    Return: It returns true if it founds thr character at the end of string
    Example:

    ```js
    const str1 = "Cats are the best!";
    console.log(str1.endsWith("best", 17)); // output: true
    const str2 = "Is this a question";
    console.log(str2.endsWith("?")); // expected output: false
    ```

9.  `includes`
    Parameters: two parameters searchString and position(optional). The includes() method performs a case-sensitive search to determine whether one string may be found within another string, returning true or false as appropriate.
    Return: returs true or false accordingly.
    Example:

    ```js
    "Cats are the best!".includes("Cats"); //true
    const sentence = "The quick brown fox jumps over the lazy dog.";
    const word = "fox";
    console.log(
      `The word "${word}" ${
        sentence.includes(word) ? "is" : "is not"
      } in the sentence`
    ); // output: "The word "fox" is in the sentence"
    ```

10. `indexOf`
    Parameter: Accepts two parameter searchValue and fromIndex(optional). seraches the index number of a given string.
    Return: returns index of searchValue otherwise gives -1 as default if not found.
    Example:

    ```js
    "hello world".indexOf("d"); //10
    "hello world".indexOf("", 8); // 8 Because an empty searchValue parameter and fromIndex value more than 0 returns the fromIndex value.
    ```

11. `lastIndexOf`
    Parameter: Accepts two parameter searchValue and fromIndex(optional).
    Return: Returns index of last occurence of searchvalue.
    Example:

    ```js
    const paragraph =
      "The quick brown fox jumps over the lazy dog. If the dog barked, was it really lazy?";
    const searchTerm = "dog";
    console.log(
      `The index of the first "${searchTerm}" from the end is ${paragraph.lastIndexOf(
        searchTerm
      )}`
    ); //output: "The index of the first "dog" from the end is 52"
    ```

12.`padEnd`
Parameter:The padEnd() method pads the current string with a given string (repeated, if needed) so that the resulting string reaches a given length. The padding is applied from the end of the current string. It accepts two parameters. targetLength and padStrings.
Return: It returns a String of the specified targetLength with the padString applied at the end of the current str.
Example:

```js
"abc".padEnd(10); // "abc       "
"abc".padEnd(10, "foo"); // "abcfoofoof"
```

13.`padStart`
Parameter: The padStart() method pads the current string with another string (multiple times, if needed) until the resulting string reaches the given length. The padding is applied from the start of the current string.
Return: A String of the specified targetLength with padString applied from the start.

```js
"abc".padStart(10); //output "       abc"
"abc".padStart(10, "foo"); // output "foofoofabc"
```

14.`repeat`
Parameter: It accepts count parameter.
Return: It returns a new string containing the specified number of copies of the given string.
Example:

```js
"abc".repeat(2); //output 'abcabc'
"abc".repeat(3.5); // output 'abcabcabc' (count will be converted to integer)
```

15.`replace`
Parameter: The replace() method returns a new string with some or all matches of a pattern replaced by a replacement. The pattern can be a string or a RegExp, and the replacement can be a string or a function to be called for each match. If pattern is a string, only the first occurrence will be replaced. The original string is left unchanged.
It accepts parameters such as regexp (pattern), substr, newSubstr (replacement), replacerFunction (replacement).
Example:

```js
const p =
  "The quick brown fox jumps over the lazy dog. If the dog reacted, was it really lazy?";
console.log(p.replace("dog", "monkey")); // output: "The quick brown fox jumps over the lazy monkey. If the dog reacted, was it really lazy?"
```

16.`slice`
Parameter: The slice() method extracts a section of a string and returns it as a new string, without modifying the original string. It accepts parameters like beginIndex and endIndex(optional).
Return: It returns a new string containing the extracted section of the string.
Example:

```js
const str = "The quick brown fox jumps over the lazy dog.";
console.log(str.slice(31)); // output: "the lazy dog."

"The morning is upon us.".slice(1, 8); //output 'he morn'
```

17.`split`
Parameters: The split() method divides a String into an ordered list of substrings, puts these substrings into an array, and returns the array. The division is done by searching for a pattern; where the pattern is provided as the first parameter in the method's call. It accepts two parameters such as separator and limit, both are optional.
Return: An Array of strings, split at each point where the separator occurs in the given string.
Example:

```js
const str = "The quick brown fox jumps over the lazy dog.";
const words = str.split(" ");
console.log(words[3]); //  output: "fox"
```

18.`substring`
Parameter: The substring() method returns the part of the string between the start and end indexes, or to the end of the string. It accepts two parameters indexStart and indexEnd(optional).
Return: A new string containing the specified part of the given string.
Example:

```js
const str = "Mozilla";
console.log(str.substring(1, 3)); //  output: "oz"
```
