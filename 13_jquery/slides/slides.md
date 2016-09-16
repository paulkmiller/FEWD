##Agenda

* JavaScript Questions
* jQuery

---

##JavaScript Questions

I know you've got em

---

##jQuery

jQuery __is__ JavaScript

---

##jQuery

jQuery is a cross-browser JavaScript library designed to simplify the client-side scripting of HTML.

The jQuery library provides the jQuery function, which lets you select elements using CSS selectors.

---

##jQuery

* [jquery.com](jquery.com) - A JavaScript library that makes DOM manipulation simple.

* Cross browser - works the same in all* browsers.

* Allows:
  * Document traversal
  * CSS Manipulation
  * Event Handling
  * Animation
  * and more!

---

##jQuery

Adding jQuery to your website

<br/>
<small>&lt;script src="js/jquery-1.11.1.min.js"&gt;&lt;/script&gt;</small>

<small>&lt;script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"&gt;&lt;/script&gt;</small>

---

##jQuery Syntax

###$

The Dollar Sign

--

##jQuery Syntax

###$

```
var listItems = jQuery( 'li' );

var listItems = $( 'li' );
```

```$``` is a shorter, more convenient name for the ```jQuery``` function

---

##jQuery Selectors
Finding elements on a page, use selectors with the $ function:

```
$('#top');  // select the element with an ID of 'top'
$('li');    // select all list items
$('ul li'); // select all unordered list items
$('.hero'); // select all elements with a class of 'hero'
```

Returns HTML elements you have selected.

--

##jQuery Selectors

Selectors are just like CSS

```
document.getElementById('myElement');
// WITH JQUERY BECOMES
$('myElement');
```

---

##jQuery Events

```
function clickHandler(event){
  console.log('you clicked!');
}

document.getElementById('myElement').onclick = clickHandler;
// WITH JQUERY BECOMES
$('#myElement').click(clickHandler);
```

--

##jQuery Events

```
$( 'li' ).click(function( event ) {
  console.log( 'clicked', $( this ).text() );
});
```

In an event handler, "`this`" will represent the thing that triggered the event.
In this case, it's the `li` that was clicked on.

Passing `this` to `$` lets you do jquery-ish things to the element.

--

##jQuery Events

```
$( 'li' ).on( 'click', function( event ) {
  console.log( 'clicked' );
});
```

When using the ```.on()``` method, you pass the native event name as the first argument, and then the handler function as the second argument.

--

##jQuery

###Some available event shortcuts

```
.click()
.keydown()
.keypress()
.keyup()
.mouseover()
.mouseout()
.mouseenter()
.mouseleave()
.scroll()
.focus()
.blur()
.resize()
```

---

##jQuery Class Manipulation

```
$( 'li' ).addClass( 'active' );
$( 'li' ).removeClass( 'active' );

$( 'li' ).toggleClass( 'active' );
```

--

##jQuery Class Manipulation

```
<div class="something">Some text.</div>
```

$( '.something' ).toggleClass( "active" )

```
<div class="something active">Some text.</div>
```

---

##jQuery Data

Data stored in your markup can be accessed using jQuery

```
<div id="person" data-name="Wilbur"></div>
```

```
var name = $('#person').data('name');
console.log(name);
// Wilbur
```

---

##jQuery Effects

```
$( '.things' ).show();
```
Will cause all `.things` to become visible

--

##jQuery Effects

```
$( '.things' ).show( 300 );
```
Will animate the 'show' action over 300 milliseconds

--

##jQuery Effects

```
.show()
.hide()
.fadeIn()
.fadeOut()
.slideDown()
.slideUp()
.slideToggle()
```

---

##jQuery

Everything you need to know is here:

###http://jquery.com
###http://learn.jquery.com

---

##Good night!

<img src="../img/unit_2/it_crowd_dancing.gif">
