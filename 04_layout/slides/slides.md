##Agenda

*	Review
*	HTML5 Structural Elements
*	Floats
*   Display Modes
*	Lab Time

---

##Review

What would you like to review?

---

##HTML5 Structural Elements

Adding structure to HTML elements that are related to content.

*	header
*	nav
*	section
*	aside
*	footer

---


##Floats

Float is a CSS positioning property, used to layout a web page.

![](http://css-tricks.com/wp-content/csstricks-uploads/web-layout.png)

Note:
Image from Chris Coyier's CSS-Tricks

---

##Floats (Benefits/Uses)

* Make line-wrapping content very easy.
* Easily align left and right sides of the columns to the container.
* Ability to reverse the order of the floated items with float: right or float: left.
* Fully supported in all browsers.

---

##Floats (Disadvantages)

* Floated elements don't honor relative height. ([Zero-Height Container Problem](http://complexspiral.com/publications/containing-floats/))
* Requires clearfix CSS to maintain content flow.
* A considerable amount of CSS is required just to adjust alignments.

---

##Clearfix

Allows elements to clear themselves

```
.clearfix:after {
  content: "";
  display: table;
  clear: both;
}
```

---

![GeneralAssemb.ly](../img/icons/code_along.png)
##Floating Sections

---

##Display Modes

Setting `display` on an element will also change layout

* `display:inline;`
* `display:block;`
* `display:inline-block;`

--

##Display Modes

###Inline

<span style="background:white; color:black; margin:20px; padding:5px; width:60%;">An `inline` element</span> has no line break before or after it, and it tolerates HTML elements next to it.

<br>

* respects left & right margins and padding, but not top & bottom
* cannot have a width and height set
* allow other elements to sit to their left and right.

--

##Display Modes

###Block

<div style="background: white; color: black; margin: 20px auto; padding: 5px; width: 60%;">A block element</div> has some whitespace above and below it and does not tolerate any HTML elements next to it.

<br>

* respect all the margins and padding
* forces a line break

--

##Display Modes

###Inline-Block

<div style="display:inline-block; background: white; color: black; margin: 20px auto; padding: 5px; width: 230px;">An inline-block element</div> is placed as an inline element (on the same line as adjacent content), but it behaves as a block element.

<br>

* allow other elements to sit to their left and right
* respect top & bottom margins and padding
* respect height and width

---

##The Future: Flexbox

* CSS for Flexbox is easy to write
* We have true vertical and horizontal centering (no more margin: auto)
* [Browser Adoption](http://caniuse.com/flexbox)
* [See Stephen Hay's Flexbox Tutorial](http://www.creativebloq.com/netmag/create-slick-css-layouts-flexbox-41411325)
