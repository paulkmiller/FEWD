##Agenda

* Questions
* JS Syntax
* Variables
* Conditionals
* Lab Time

---


##Questions

Hello! Ask me questions!

---

##JS Syntax

__Syntax:__ Spelling and grammar rules of a programming language.

Common syntax elements of javascript:

* Semicolon
* Brackets
* Curly Braces
* Parentheses

--

##JS Syntax

#### Semicolon

Every statement in javascript should be finished with a semicolon. They are like the period at the end of a sentence.

```
var thisThing = 'some words';
```

--

##JS Syntax

#### Brackets

Brackets are used to access data (more on that later)

```
var thing = list[0]; /* gets the first item in the list */
```

--

##JS Syntax

#### Curly Braces

Curly Braces are used to group a set of statements together based on some preface (eg: an `if` statement, or a `function`)

```
if(thisThing == true) {
  var thing = 'another thing';
  doSomething();
}
```

--

##JS Syntax

#### Parentheses

Parenthesis are used to group operations (generally math or logic), or to "call" a function (to make it run).

```
if( (thisThing && thatThing) || veryImportantThing ) {
  doSomething();
}

```

---

##Variables

* We can tell our program to remember values for us to use later on.

* The action of saving a value to memory is called assignment

* The entity we use to store the value is called a variable

* The action of getting the value from a variable is called accessing the variable

--

##Variables Declaration

We can declare and assign separately or together.

Declaration: ```var age;```

Assignment: ```age = 21;```

Both at the same time: ```var age = 21;```

--

##Variable Re-Assignment

```var name = 'Jo';```

```name = 'Amir';```

The value of `name` is now `'Amir'`


--

##Variable Conventions

* Variables start with a lower case letter

* If they contain multiple words, subsequent words start with an upper case letter (camel casing)

`var numberOfStudents = 10;`

---

##Variables & Data Types

What can you store in a variable?

--

##Data Types

Some of the types of values we support include:

* __String__ text
* __int__, __float__ numbers
* __Boolean__ true or false

---


![GeneralAssemb.ly](../img/icons/code_along.png)
##Score Keeper

[Score Keeper CodePen](http://codepen.io/paulkmiller/pen/yaNGOJ)

---

##Strings

* Stores textual information
* String literal is surrounded by quotes
<br/><br/>
```'How is the weather today?'```
<br/><br/>

Single quotes are considered best practice.

--

##Strings

Double vs single quoted strings:

'They "purchased" it'

"It's a beautiful day"

--

##Strings
Escaping
"They \"purchased\" it"

'It\'s a beautiful day'

---

##Conversion: String To Number

```
var intString = "4";
var intNumber = parseInt(intString, 10);
var floatString = "3.14159";
var floatNumber = parseFloat(floatString);
```

Note:
Why would you need to convert datatypes?

---

##Conversion: Number To String

```
var number = 4;
number.toString(); /* => "4" */
```

__OR__
```
number + ""; /* => "4" */
```

Note:
Why would you need to convert datatypes?

---

##Numbers

Represent numerical data

int:         42

float:      3.14159265

--

##Numbers

With signs

int:         +6

float:      -8.2

Can perform arithmetic on number data types

---


##Arithmetic In JavaScript

![](../img/unit_1/arithmetic.jpg)

---

##Conditionals

![](../img/unit_1/cfDiagram.png)

---

##Making Decisions

It's either TRUE or FALSE (booleans)

If your age is greater than 18 you are an adult

```
  if (age > 18){
    document.write("You are an adult");
  }
```

---

##Comparisons - Equality

Are two things equal?

```
10 === 10 //true
10 === 5 //false
"hi" === "hi" //true
```
---


##Logical Operators

![](../img/unit_1/logical_operators.png)

---

##Conditional Syntax

```
if(condition is true) {
  //Do cool stuff
}
```

--

##Conditional Syntax

```
  if(condition is true) {
    //Do cool stuff
  }else{
    //Do other cool stuff
  }
```

--

##Conditional Syntax

```
  var topic = "JS";

  if (topic == "JS") {
    console.log("You're learning JavaScript");
  }
  else if(topic == "JavaScript") {
    console.log("You're still learning JavaScript");
  }
  else {
    console.log("You're learning something else");
  }
```

---

##Multiple Conditions

```
if (name == "GA" && password == "YellowPencil"){
  //Allow access to internet
}
```

---


##The Truth Table

```
if (name == "GA" && password == "YellowPencil"){
  //Allow access to internet
}
```

--

##The Truth Table

![](../img/unit_1/and_table.png)

--

##The Truth Table

```
if (day == "Tuesday"  || day == "Thursday"){
  //We have class today
}
```

--

##The Truth Table

![](../img/unit_1/or_table.png)

---

##The Console

A debugging tool, used to give yourself information about something in your code.

```
console.log("This text goes in the console of your inspector!");
```

---

![GeneralAssemb.ly](../img/icons/code_along.png)
##Light Switch

[Light Switch CodePen](http://codepen.io/paulkmiller/pen/rrVoZW)

---

![Temp Converter](../img/icons/exercise_icon_md.png)
##Temp Converter

[Temp Converter CodePen](http://codepen.io/paulkmiller/pen/kkWzbg)

---

##Good night!

<img src="../img/unit_2/space_bear.gif">
