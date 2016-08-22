##Agenda

* Review
* Box Model
* Nested Selectors
* Class & ID
* Lab Time

---

##Review

What do you need help with?

---

##CSS Placement

Where can CSS go?

* Inline
* In the `head`
* *In a separate file*


Note:
CSS should go in a separate file. We're going to start by placing them in the head for convenience and to learn the syntax. We'll show inline styles at the end, just to demonstrate.

--

##CSS Placement

###Inline

```<p style="color:red; font-weight:bold;"></p>```

--

##CSS Placement

###In the `head`

```
<head>
  <style>
    p {
      color: red;
      font-weight: bold;
    }
  </style>
</head>
```

--

##CSS Placement

###Using a separate CSS file

####This is best practice!

```
  <head>
    <link rel="stylesheet" href="style.css">
  </head>
```

Note:
"The `link` tag needs two attributes: `rel="stylesheet"` and an `href` attribute.

The `href` attribute value works very similarly to linking to an image, or to another page.


---

##CSS Break Down

```
p {
  color: red;
  font-weight: bold;
}
```
--

##CSS Break Down

This whole thing is called a **rule**.

The `p` is called a **selector**, and it's followed by a set of **declarations** in a **declaration block**.

```
p {
  color: red;
  font-weight: bold;
}
```

--

##CSS Break Down

The **selector**, `p` in this case, specifies what parts of the HTML document should be styled by the declaration. This selector will style all `p` elements on the page.

```
p {
  color: red;
  font-weight: bold;
}
```

--

##CSS Break Down

The **declaration block** here is:

```
{
  color: red;
  font-weight: bold;
}
```

**Declarations** go inside curly braces.

--


##CSS Break Down

#### Declarations

This example has two declarations. Here's the first:

```
color: red;
```

Note:
Every declaration is a **property** followed by a **value**, separated by a colon, ending in a semicolon.

In this declaration, we are setting the `color` **property** to the **value** `red`.


--


##CSS Break Down

Let's look at the second declaration:

```
font-weight: bold;
```

Note:

What style **property** are we specifying here?

What **value** are we setting that **property** to?

Try writing a new set of styles for another element, like an `h1`.


--

##CSS Break Down

Why might we want to link to a separate CSS file?

Note:

Discuss as a class


---

##CSS Colors

Colors can be specified in CSS in a variety of ways:

![](../img/unit_1/color.png)

Note:
* keyword
* hex codes
* rgb
* hsl
* rgba
* hsla

--

##CSS Colors
###Color Keywords

These are used less frequently, but are handy for `black` and `white`.

See [here](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value) for more

--

##CSS Colors
###Hex Codes (RGB)

![Hex Color explanation](../img/unit_1/hex_colors.png)

Note:
"Hex" values are so-called because they use hexadecimal, or base-16, to describe the color values for red, green, and blue. Each of the 3 color values is expressed by two hexadecimal digits, from `00` (no color) to `FF` (full color), and are written in the order red, green, then blue, after an initial `#` sign.

Hex values can be abbreviated to only 3 digits if each digits is doubled. So `#FFFFFF` (white) can be expressed more succinctly as `#FFF`, and `#000000` (black) can be expressed as `#000`. `#FA6198`, however, cannot be abbreviated without altering the color.

--

##CSS Colors
###RGB Color Values

####```rgb(0,0,0)```

* The first value is red, the second green, the third blue.

* Each value can range from 0 to 255, which expresses the same number of color steps as 00 to FF in base-16.


Note:
FF in base-16 is equivalent to 255 in base-10.

In RGB, `rgb(0,0,0)` is black, `rgb(255,255,255)` is white, `rgb(255,0,0)` is red, etc.

White-space is allowed *inside* the parentheses, so `rgb(255, 0, 0)` will do just as well.
</aside>

--

##CSS Colors
###RGBa Colors


* RGBa works identically to RGB, expect that it takes a 4th value called the "alpha".
* This is a value between 0 and 1 which will be used to determine a color's opacity on the page


![](../img/unit_1/rgba_color.png)

Note:
0 is completely transparent, and 1 being solid. 0.5 or .5 is 50% opacity.

Thus, __rgba(0,0,0,.25)__ is black at 25% opacity and __rgba(255, 255, 255, 0.8)__ is white at 80% opacity.

The alpha value can be in decimal form but cannot use a percentage. When a decimal is used, the leading zero is optional.

--

##CSS Colors
###HSL Colors (uncommon)

####HSL
* Similar notation to RGB values, but specify colors using hue, saturation, and lightness.

####HSLa
* As with RGBa, HSLa is exactly like HSL for the first 3 values, but takes a 4th alpha-channel value.

Note:
**Hue** is expressed as a degree angle measure, with red being at 0, green at 120, and blue at 240. Note that the degree unit is implied, and that the angle wraps around, so 360 also refers to red, and -120 is the same as 240 (blue).

**Saturation** is expressed as a percentage, with 100% being a fully saturated color, and 0% being a shade of gray (no hue).

**Lightness** is also expressed as a percentage, 0% being black, and 100% being white. 50% lightness is the "normal" color range: anything above 50% gives a white tint, anything below 50% gives a black shade.

As an example, red is ```hsl(0, 100%, 50%)```, which is equivalent to ```#FF0000```.

Note that changing the opacity allows whatever colors are "behind" an element to shine through, which can alter the visible color significantly, especially at lower opacities.

---


##Box Model

Every element in web design is a box.

--

##Two Kinds of Boxes

###Block Elements - They're Greedy

They will take up the entire width of their containers. They want the entire line to themselves.


###Inline Elements - They're Clingy

They will sidle up to neighboring elements in a horizontal line. They want to share lines with others.

--

##Box Model

4 compontents: margin, border, padding and (content) width/height

![](http://www.mandalatv.net/itp/drivebys/css/lib/img/box_model.gif)

--

##Box Model

```
article{
  border: 5px solid #000;
  height: 500px;
  margin: 20px;
  padding: 20px;
  width: 500px;
}

```
--

##Box Model


###Width = (content) width + padding-left + padding-right + border-left + border-right

--

##Box Sizing

That's lot's of math to find the actual width and height...

###enter box sizing.

width = actual visible/rendered width of box

height = actual visible/rendered height of box

```
html {
  box-sizing: border-box;
}
*, *:before, *:after {
  box-sizing: inherit;
}
```

---

##Nested Selectors

Styling just the stuff we want to

--

##Nested Selectors

```
<p>
  <span>red</span>
  <div>green
    <span>blue</span>
  </div>
</p>
```

We need to target each of these to make them the right color

--

##Nested Selectors

```
<p>
  <span>red</span>
  <div>green
    <span>blue</span>
  </div>
</p>

p { color: white; }

```

<span style="color:white;">red <br>green blue</span>

--

##Nested Selectors

```
<p>
  <span>red</span>
  <div>green
    <span>blue</span>
  </div>
</p>

p { color: white; }
p span { color: red; }

```

<span style="color:white;"><span style="color:red;">red</span> <br>green <span style="color:red;">blue</span></span>

--

##Nested Selectors

```
<p>
  <span>red</span>
  <div>green
    <span>blue</span>
  </div>
</p>

p span { color: red; }
p div { color: green; }

```

<span style="color:white;"><span style="color:red;">red</span> <br><span style="color:green;">green</span> <span style="color:red;">blue</span></span>

--

##Nested Selectors

```
<p>
  <span>red</span>
  <div>green
    <span>blue</span>
  </div>
</p>

p span { color: red; }
p div { color: green; }
p div span { color:blue; }

```

<span style="color:white;"><span style="color:red;">red</span> <br><span style="color:green;">green</span> <span style="color:blue;">blue</span></span>

---

##Pseudo Selectors

```a:hover { color:#78b9e6; }```

Hover over <a>this</a> link

--

##Pseudo Selectors

```div:first-letter { font-size:200%; }```

<style>
  #large-letter:first-letter { font-size:200%; }
</style>

<div id="large-letter">First letter is large!</div>

---

##class & id

With classes and ids we can target specific elements on a page, so we can manipulate it uniquely.

--

##class & id

####IDs are unique

####Classes are not unique

--

##class & id

When should you use them?

--

##Specificity

CSS reads top-down and by specificity.

ID (more specific) > Class > Element (less specific)

---

##[Fashion Blog](class_03_starter_code/Fashion_Blog_final.png)

---

##Good night!

![](../img/unit_1/dancing_cupcake.gif)
