##Forms

How we can get data from users.

![](../img/unit_2/forms.png)

---

##Forms

<style>
.slides-margin {
  margin-left:15px;
  position:relative;
  top:-5px;
}
input {
  font-size:0.5em;
}
</style>

* Wrapper for data collection elements

  * Text fields <input class="slides-margin">
  * Dropdowns
  <select class="slides-margin">
    <option>Option A</option>
    <option>Option B</option>
  </select>
  * Radio Buttons
  <input type="radio" class="slides-margin">
  * etc

---

##Forms

Tells the page:

* Where to send the data
* How to send it
* What is being sent

----

##Form Tag

![](../img/unit_2/form_tag.png)

Available Attributes

* `method`: POST, GET, PUT, DELETE
  * This is called REST, this is how the internet works
* `action`: URL to send data to
* `enctype`: For POST only
  * Shoud set to "multipart/form-data" if uploading files

<br>
This stuff is highly dependent on how your backend has been configured

---

##Form Tag

In Action

```
<form action="register.php" method="post" enctype="multipart/form-data">
  <!--Data collection elements go here-->
</form>
```

----

##Inputs

* Place between ```<form> </form>``` tags

* Attributes
  * `type`: Text, submit, password, email, checkbox, button, radio, file, etc
  * `name`
    * Used server side
  * `placeholder`
  * `value`

Note:
Complete Spec: <https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input>

* Gotchas
  * The font-family for an input is not inherited!!!
  * This can lead to funny sizing issues on Macs vs. PCs where the default font is not the same


---


##Text

Use value to set initial text


![](../img/unit_2/text.png)

![](../img/unit_2/forms.png)

---

##Email

Allows browser to autofill field

![](../img/unit_2/email_type.png)

![](../img/unit_2/email.png)


---

##Password

Hides characters as typed

![](../img/unit_2/password_type.png)

![](../img/unit_2/password.png)

----

##Submit vs File vs Button

* Submits the form

```
<input type="submit" value="Submit">
```
<input type="submit" value="Submit"><br/>
<hr>

* Creates a file upload element

```
<input type="file">
```

<input type="file"><br/>
<hr>

* Just a button

```
<input type="button" value="A Button">
```

<input type="button" value="A Button">

----

##Select and Option

```
<select>
  <option value="1">FIRSTOPTION</option>
  <option value="2">ANOTHEROPTION</option>
</select>
```

<select>
  <option value="1">FIRSTOPTION</option>
  <option value="2">ANOTHEROPTION</option>
</select>

----

##Labels

Info about the input field should be put in a ```<label>``` tag
Clicking the label gives the input focus!

```
<label for="yourName">Enter your name:</label>
<input type="text" name="yourName" id="yourName">
<label for="coolness">Are you cool?</label>
<input type="checkbox" name="coolness" id="coolness">
```

<label for="yourName">Enter your name: </label><input type="text" name="yourName" id="yourName" class="slides-margin">
<label for="coolness">Are you cool?</label><input type="checkbox" name="coolness" id="coolness" class="slides-margin">

Note:
Usability
Clicking the label text in either case places the focus in the input field (great for radio buttons)

----

##Styling

* Can't be styled directly:
  * Checkboxes
  * File upload inputs
  * Radio buttons

Note: Number of ways to do this *instructor can cover all or just choose one
  1.  Opacity 0 on the element, set it's height and width to define clickable area, set the height and width of it's parent to be the same as the input (don't forget position relative). Style the parent.
  2.  Hide the element, style a corresponding label how you wanted the element to appear
  3.  Try using pseudo elements and the selector :checked for no JS switching between checked and unchecked images used for styling


----
# jQuery Plugins

* What are they?
* What can they be used for?

---

# jQuery Plugins

jQuery is set up in a way where developers can add new functionality via some additional javascript called a "plugin".

---

# jQuery Plugins

###What are they used for?
###Just about everything!

---

# jQuery Plugins

* Visual effects
* Navigation elements
* Analytics
* Loading data

----

# Carousel

###Slick

http://kenwheeler.github.io/slick/

----

# Scrolling

###GoUp

http://ryuk87.github.io/jquery-goup/

###Skrollr

http://prinzhorn.github.io/skrollr/

###Waypoints

http://imakewebthings.com/waypoints/

----

# Sticky

###StickyKit

http://leafo.net/sticky-kit/

###Stick Up

http://lirancohen.github.io/stickUp/
----

# Layout

###Mansonry

http://masonry.desandro.com/

###Isotope

http://isotope.metafizzy.co/

###Full Page Scroll

http://alvarotrigo.com/fullPage/
----

# What else?

###You name it!
----
##Good night!

<img src="../img/unit_2/hedgehog_cat.gif">
