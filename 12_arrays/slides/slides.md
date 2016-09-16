##Agenda

* JavaScript All Over Again
* Arrays
* querySelectorAll
* forEach

---

##Questions

---

##JavaScript, Again

JavaScript is a series of **expressions**.

Expressions are **values** (strings, numbers, booleans) combined with **operators** (+, *, %, &&, !).

```
3 + 3 // <- Expression
```

Expressions make up **statements** which cause stuff to happen.
Statements end in semi-colons!

```
var x = (54 / (2 * 3 + 4)); // <- Statement
```

---

## Functions, Again


Statements can be combined into **functions** to be used later in the code,

```
function add3(x) {       // This whole
	var result = x + 3;  // thing
	return result;       // is a
}                        // function *definition*
```
**Function definitions** don't run the code inside the
curly braces, they just set it up.


Once defined, functions can be *called*, supplying all their **arguments** inside parentheses.

```
var xyz = add3(45); // 45 fills the x argument

console.log(xyz); // <- Prints out 48 to the console.
```

---

## JavaScript + HTML, Again

```
var buttonElement = document.getElementById('myButton');
var statusElement = document.getElementById('status');

buttonElement.onclick = function () {
	statusElement.innerHTML = 'Oh wow. So click. Much JavaScript.'
}
```


---

## Arrays!

**Arrays** are "ordered lists". They have elements which are *indexed*, and they have a **length**. Arrays are "Zero-Indexed"

```
// Make an array, with "An Array Literal"
var todoList = ["Take out the trash", "Quit smoking", "Learn JavaScript"];

// Access element at index 1
console.log( todoList[ 1 ] ); // Prints out "Quit smoking"

// Get the length
console.log( todoList.length ); // Prints out 3

// Access the element at the length
console.log( todoList[ todoList.length ] ) // ALWAYS UNDEFINED!!

// Correct accessing of very last element
console.log( todoList[ todoList.length - 1 ] ) // Prints out "Learn JavaScript"
```

---

## Arrays, cont.

```
// Repeated for clarity
var todoList = ["Take out the trash", "Quit smoking", "Learn JavaScript"];

// Set the element at index 2
todoList[2] = "Learn AngularJS";

// Arrays can contain AnYtHiNg!
var badList = [234, "abcd", [], null]; // Don't do this. Ask me why.
```

---

## Arrays have functions

Arrays have lots of cool functions

```
// Repeated for clarity
var todoList = ["Take out the trash", "Quit smoking", "Learn JavaScript"];

// Join the elements together, with something in the middle.
todoList.join(', then ') // <- "Take out the trash, then Quit smoking, then Learn JavaScript"

// Find an element
todoList.indexOf("Take out the trash") // <- 0

// Reverse an array
[1, 2, 3, 4].reverse() // <- [4, 3, 2, 1]
```

---

## forEach Loop

A loop runs the same code over and over again, for a set number of times.

Arrays have a function called forEach, which loops once for each element in the array.

```
// Repeated for clarity
var todoList = ["Take out the trash", "Quit smoking", "Learn JavaScript"];

// For each element in the array...
todoList.forEach(function (listItem, index) {
	// Print it out, with its index
	console.log("Item #" + index + ": " + listItem )
})

```

---

## When and why Arrays?

* You have a number of similar things
* You have items that are ordered

---

## querySelectorAll

Use CSS-like selectors to get a *list* (read: array) of elements. The list is in the order that the elements appear in the HTML. Unfortunately, it's a fake array. Fortunately, jQuery solves this problem.

```
var allAElements = document.querySelectorAll('a');

allAElements[0] // Works perfectly, returns the first link on the page

allAElements.forEach(myLoopingFunction) // <- Error, forEach is undefined.

// Problem solved, but this looks really weird...
[].forEach.call(allAElements, myLoopingFunction)

```


---

![GeneralAssemb.ly](../img/icons/code_along.png)
## Fun With Spans

[Fun with Spans Starter Code](../12_arrays/class_12_fun_with_spans_starter_code.zip)

---

## Homework

Interactive Story Blog or Rewrite Fun with Spans solution code

---

##Good night!

<img src="../img/unit_2/beard_slap.gif">
