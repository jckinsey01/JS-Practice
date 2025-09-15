# Describe Me - A Lesson on Data Types

![Cute bunch of 4 kittens](./../assets/images/cute-kittens.jpg)

Let's pause for a second and make sure that we understand how data are another way to describe our reality. Different types of data and data structures offer us different ways to carry out this descriptive work.

In small groups of 3-4 people, work through the following sections that ask you to describe the above image of kittens with different types of data primitives and data structures.

<p class="warning">
  Be sure to render your variables to the page in a separate codeblock, so you know the code is working.
</p>

## 1. String

Create a variable that is assigned a String that describes this image in 1-2 sentences.

```js
let cuteKittens = "a group of four very cute kittens, three tabbies and one orange!";
```
```js
console.log(cuteKittens);
```

## 2. Array

Create a variable that is assigned to an Array that has 4 or more values to describe this image.

```js
const kittenArray = ["tabby 1", "tabby 2", "tabby 3", "orange guy"];
```

```js
console.log(kittenArray);
```

## 3. Object

Create a variable that is assigned 1 object with at least 4 key-value pairs.

```js
let orangeGuy = {
  name: "Leaf",
  color: "orange tabby",
  eyeColor: "blue",
  favoritefood: "tuna",
};
```

```js
console.log(orangeGuy);
```

## 4. Array of Objects

Create a variable that is assigned an Array with 4 objects that represent each kitten. Make sure that each kitten object shares the same keys.

```js
let kittenGroup = [
  {
    name:"Bobby",
    color:"Tabby",
    eyeColor:"Blue",
    favFood:"Yogurt",
  },
  {
    name:"Timmy",
    color:"Tabby",
    eyeColor:"Blue",
    favFood:"Blueberries",
  },
  {
    name:"Tommy",
    color:"Tabby",
    eyeColor:"Blue",
    favFood:"Bread",
  },
  {
    name:"Leaf",
    color:"Orange Tabby",
    eyeColor:"Blue",
    favFood:"Tuna",
  },
];
```

```js
kittenGroup
```

## Helpful Transformative Methods in JS

We should remember a few useful methods, when working with the above types of data. Let's practice some of them together:

### Strings

```js
/**
 * Strings:
 * concatenation, .charAt(), .slice(), .split()
**/
cuteKittens.split(" ")
```



### Arrays

```js
/**
 * Arrays:
 * Using index position, .push(), for loops, .map()
**/
for (let kitty in ) {
console.log(kitty);
}
```


### Objects

```js
/**
 * Objects:
 * Accessing values with keys; Adding new properties (key-value pairs)
**/
orangeGuy.name
```

### Array of Objects

```js
/**
 * Array of Objects:
 * Looping through and accessing properties with keys;
 * Adding new props;
 * Difference between .map() and for loops
**/
let newKittenGroup = kittenGroup.map(
  (kitty) => {
    if (kitty.color == "Orange Tabby") {
      return "Crazy guy!"
      return kitty
    }
    else if (kitty.color == "Tabby") {
      return "Suave guy!"
      return kitty
    }
  }
)
```
