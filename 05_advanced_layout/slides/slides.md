##Agenda

*	Questions?
* Resets
*	Overflow
*	Box Sizing
*	Lab Time

---

##Questions?

Hey, do you have any questions?

---

##CSS Resets

--

##CSS Resets

###Why do we need them?

* Browsers don't all use the same default styles (I'm looking at you, Internet Explorer)
* Resets give us a consistent starting point

--

##CSS Resets

Which one should I use?

* Any of the ones at http://www.cssreset.com/
* I prefer http://necolas.github.io/normalize.css/


---

<style>
  .reveal div.overflow-demo {
    background:rgba(255,255,255,.25);
    color:white;
    height:70px;
    width:50%;
    margin:auto;
  }
</style>

##Overflow

--

##Overflow

Changes the way that the page deals with content that goes outside of the width and/or height defined for an element.


####<div style="margin-top:30px;">For Example</div>

* Images that "bleed" out for visual effect
* Sections of the page that need to scroll

--

##Overflow
#### examples at ```height:70px;```

```overflow: visible;```

<div class="overflow-demo" style="overflow:visible;">This text is going to be visible outside of the box</div>

--

##Overflow
#### examples at ```height:70px;```

```overflow: hidden;```

<div class="overflow-demo" style="overflow:hidden;">This text is going to be hidden outside of the box</div>

--

##Overflow
#### examples at ```height:70px;```

```overflow: scroll;```

<div class="overflow-demo" style="overflow:scroll;"><div style="width:600px">This text is going to be scrollable both vertically and horizontally</div></div>

```overflow-y: scroll;```

<div class="overflow-demo" style="overflow-y:scroll;">This text is going to be vertically scrollable</div>

```overflow-x: scroll;```

<div class="overflow-demo" style="overflow-x:scroll; overflow-y:hidden;"><div style="width:900px">This text is going to be horizontally scrollable</div></div>

--

##Overflow
#### examples at ```height:70px;```

```overflow: auto;```

<div class="overflow-demo" style="overflow:auto;">This text is fine</div>

```overflow: auto;```

<div class="overflow-demo" style="overflow:auto;">This text will show a scroll bar since it is longer</div>

---

##Box Sizing

--

##Box Sizing

####`box-sizing: content-box;`

This is what you've seen so-far, the `width` and `height` only apply to the content area

<div style="background: rgba(255,255,255,.25); position:relative;">
  <div style="width:50%; border:20px solid rgba(255,0,0,.25); z-index:20; position:relative; color:white;">
    ```width:50%; padding:20px;```
  </div>
  <div style="width:50%; height:100%; position:absolute; background: rgba(255,255,255,.25); z-index:10; top:0; right:0;"></div>
</div>

--

##Box Sizing

####`box-sizing: border-box;`

The `width` and `height` include `padding` and `border`

<div style="background: rgba(255,255,255,.25); position:relative;">
  <div style="width:50%; border:20px solid rgba(255,0,0,.25); z-index:20; position:relative; color:white; box-sizing:border-box;">
    ```width:50%; padding:20px;```
  </div>
  <div style="width:50%; height:100%; position:absolute; background: rgba(255,255,255,.25); z-index:10; top:0; right:0;"></div>
</div>

---


![GeneralAssemb.ly](../img/icons/exercise_icon_md.png)
##Fashion Blog Part 2

---

##Good night!

<img src="../img/unit_1/gorillaz.gif" width="500px">
