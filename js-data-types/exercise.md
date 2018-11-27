# Javascript Data Types Exercises

> This worksheet will double as Javascript notes for future reference! Copy it into your preferred note-taking program at the end of class.

## Data Types

For each expression, predict what you think the output will be in a comment (`//`) ***without first running the command***. Then run the expression in the console. Note the actual output in a comment and compare it with your prediction.

#### Example

```js
typeof("potato")
// Prediction: Vegetable
// Actual: String
```

What is the output of each of the expressions below?

```js
typeof(15)
// Prediction:
// Actual:number

typeof(5.5)
// Prediction:
// Actual:number

typeof(NaN)
// Prediction:
// Actual: number

typeof("hello")
// Prediction:
// Actual: string

typeof(true)
// Prediction:
// Actual: boolean

typeof(1 != 2)
// Prediction:
// Actual: boolean


"hamburger" + "s"
// Prediction:
// Actual: hamburgers

"hamburgers" - "s"
// Prediction: hamburger
// Actual: NaN

"1" + "3"
// Prediction:
// Actual: 13

"1" - "3"
// Prediction: NaN
// Actual:-2

"johnny" + 5
// Prediction:
// Actual: johnny5

"johnny" - 5
// Prediction:
// Actual: NaN

99 * "luftbaloons"
// Prediction:
// Actual: NaN
```

What's going on in the second half of the previous question? Are there any "rules" we can pull from those examples?

## Data Structures

> Data structures include arrays and objects. We will go over objects in a later class.

### Arrays

Javascript provides us with a number of native methods that allow us to interact with arrays. Find methods that do each of the following and provide an example...
* Add an element to the back of an array.
* Remove an element from the back of an array.
* Add an element to the front of an array.
* Remove an element from the front of an array.
* Concatenates all the elements in an array into a string.
* Separates the characters of a string into an array. This one is a string method.

> This is a great exercise for practicing your "Google Fu"! If you need a starting point, check out [MDN's documentation page on arrays](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).

```js
/*
Qn: Adding an element to the back of an array
Ans: array.push("element");
Qn: Removing an element from the back of an array
Ans: array.pop("element");
Qn: Adding an element to the front of an array
Ans: array.unshift("element");
Qn: Removing an element from the front of an array
Ans: array.shift();
Qn: Concatenate all the elements in an array into a string
Ans: array.join();
Qn: var str = "How are you doing today?"
var res = str.split(separator - e.g. " "),limit (e.g. 3) )

*/

```

What will the contents of the below arrays be after the code samples are executed? Come up with an answer yourself before testing it out in the console.

```js
var numbers = [2, 4, 6, 8]
numbers.pop()
numbers.push(10)
numbers.unshift(3)
```

```text
var numbers = [3, 2, 4, 6, 10]
```

What is the return value of the below code sample? Come up with an answer yourself before testing it out in the console.

```js
var morse = ["dot", "pause", "dot"]
var moreMorse = morse.join(" dash ")
moreMorse.split(" ")
```

```text
moreMorse = ["dot", "dash", "pause", "dash", "dot", ]
```

What will the contents of the below array be after the below code sample is executed? Come up with an answer yourself before testing it out in the console.

```js
var bands = []
var beatles = ["Paul", "John", "George", "Pete"]
var stones = ["Brian", "Mick", "Keith", "Ronnie", "Charlie"]
bands.push(beatles)
bands.unshift(stones)
bands[bands.length - 1].pop()
bands[0].shift()
bands[1][3] = "Ringo"
```

```text
0: (4) ["Mick", "Keith", "Ronnie", "Charlie"]
1: (4) ["Paul", "John", "George", "Ringo"]
```
Look up and use the `delete` keyword with phoneBook to delete a record.

### Objects
```
var phoneBook = {
  "Abe": "111-111-1111",
  "Bob": "222-222-2222",
  "Cam": "333-333-3333",
  "Dan": "444-444-4444",
  "Ern": "555-555-5555",
  "Fry": "111-111-1111",
  "Gil": "222-222-2222",
  "Hal": "333-333-3333",
  "Ike": "444-444-4444",
  "Jim": "555-555-5555",
  "Kip": "111-111-1111",
  "Liv": "222-222-2222",
  "Mia": "333-333-3333",
  "Nik": "444-444-4444",
  "Oli": "555-555-5555",
  "Pam": "111-111-1111",
  "Qiq": "222-222-2222",
  "Rob": "333-333-3333",
  "Stu": "444-444-4444",
  "Tad": "555-555-5555",
  "Uwe": "111-111-1111",
  "Val": "222-222-2222",
  "Wil": "333-333-3333",
  "Xiu": "444-444-4444",
  "Yam": "555-555-5555",
  "Zed": "111-111-1111"
};
```

Write a line of code that accesses the phone number for Pam.

//console.log(phoneBook["Pam"]);

Write a line of code that creates a new record for John at 435-567-1223.

//phoneBook.push({"John":"435-567-1223"}); --> does not work for key:value in array
//phoneBook.John = "435-567-1223"; -- > dot notation or bracket notation

Write your own object and console.log that value.
//phoneBook["Wonky"] = "123-456-7890";
//console.log(phoneBook["Wonky"]);

Find out what `Object.keys(phoneBook)` does.
//It displays the keys in the array.

## Booleans & Comparison Operators

Here's an example truth table for the `!` (not) operation. In it, we're listing the values of `!a` that correspond with a given value of `a`.

|a|!a|
|---|---|
|true|false|
|false|true|

Fill out the truth tables below for `&&` (and), `||` (or) and one that uses multiple comparison operators. All you need to do is replace the `?`'s with either `true` or `false`.

> **NOTE:** Because of markdown formatting, `||` and `&&` have been replaced with `OR` and `AND` respectively.
>
> **HINT:** With the last one, it may be helpful to add additional columns to the table for each individual comparison.

| a | b | a AND b |
| --- | --- | --- |
| true | true | True |
| true | false | False |
| false | true |False |
| false | false | False |

|a|b|a OR b|
|---|---|---|
|true|true|True|
|true|false|True|
|false|true|True|
|false|false|False|

|a|b|a `!=` b|
|---|---|---|
|3|3|False|
|1|5|True|
|2|"2"|False|

|a|b|!a AND (a OR b)|
|---|---|---|
|true|true|false|
|true|false|false|
|false|true|true|
|false|false|true|

## Conditionals

You're a bouncer at a bar. Given an `age` variable, create a conditional that satisfies the following requirements...
* If a patron is older than `21`, print out `"Come on in!"`.
* If a patron is between `18` and `21`, print out `"Come on in (but no drinking)!"`.
* If a patron is younger than 18, print out `"You're too young to be in here!"`.
* If a patron is older than 75, print out `"Are you sure you want to be here?"`.

```js
/**

var age = 25;

if (age > 75) {
    console.log("Are you sure you want to be here?");
} else if (age >= 18 && age <= 21) {
    console.log("Come on in (but no drinking)!");
} else if (age < 18) {
    console.log("You are too young to be in here!");
} else {
    console.log("Come on in.");
};
**/
```

#### Bonus

Bar patrons must have an ID if the bouncer is even going to consider what age they are.
- If the patron has an ID, the bouncer will then check if they are of the proper age
- If the patron does not have an ID, the bouncer will tell them `"No ID, no entry."`

> Hint: Whether the patron has an ID or not can be stored in a `hasId` variable. What do you think the stored data type should be?

/**

var hasId = true;
var age = 25;

if (hasId === true) {
    if (age > 75) {
        console.log("Are you sure you want to be here?");
    } else if (age >= 18 && age <= 21) {
        console.log("Come on in (but no drinking)!");
    } else if (age < 18) {
        console.log("You are too young to be in here!");
    } else {
        console.log("Come on in.");
    }
} else {
    console.log("Come back with your ID");
}