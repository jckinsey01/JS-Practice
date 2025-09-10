# Gettin' Funcky with Strings

Here's what you should understand by the end of the midterm. You should know ...

1. the basics about how variable assignment and scoping works in JS;
2. the differences between JS primitives, such as Strings, Arrays, Numbers, and Objects;
3. how to use loops and conditional statements;
4. how you can nest loops and conditional statements;
5. how to convert certain data types

## Attach the dataset

Use Observable's `FileAttachment()` to attach the `pb.txt` file with the `.text()` function.

**QUESTIONS**: 

1. What data type does your attached `pb.txt` file become?
2. How many characters are in the `pb.txt` file? HINT: Use the `.length` method.
```js
const pb = FileAttachment("./../data/pb.text").text;
console.log(pb.length);
```
## Counting Matched Strings

**Data to use**: `pb.txt`

Write a function that will:

1. Split a large String by a single whitespace;
2. Use an input String, e.g., `"basketball"`, to match against Strings in the split String; and
3. Return the total amount of matches as Number.

```js
const countStringMatches = (stringData, matchString) => {
  // split the string
let splitString = stringData.split(" ")
// assign count var
let count = 0
// assign empty matches array
let matchesArray = []
//
for (const s of splitString) {
 if (s == matchString) {
console.log(s)
matchesArray.push(s)
count += 1
 }
}
// return our count
return count
}
```

```js
let splitstring = pb.split(" ")
let count = 0
for (const s of splitString) {
  if (s == "baskettball")
}
// let stringCount = splitAndCountString(pb, "basketball")
// console.log()
```
## Set of Match Info

Iterate on the previous function by writing a new function that returns a single object with the following properties:

1. Key of `keyword` with a String value of the searched for String;
2. Key of `totalMatches` with Number value of total matches found; and
3. Key of `matches` with a value of an Array that includes the matches.
4. **BONUS!** In the array of matches, create a String that also includes the String before and after the matched String:
    - EXAMPLE input of `"basketball"`:
      ```javascript
      [ "top basketball award", "womens basketball player", ... ]
      ```
```js
const countStringMatches = (stringData, matchString) => {
  // split the string
let splitString = stringData.split(" ")
// assign count var
let count = 0
let matchesArray []
for (const s of splitString) {
 if (s == matchString) {
matchesArray.push(s)
count += 1
 }
}
// return our count
return {
  keyword: matchString,
  totalMatches: count,
  matches; matchesArray,
}
}
```