# Welcome to FEWD!

---

## Hi! I'm...

* Paul Miller
* I'm a Web Developer at [Greater Washington Publishing](http://gwp2.herokuapp.com/)
* Get in touch with me at: [paulteachesweb@gmail.com](mailto:paulteachesweb@gmail.com)

---

## Agenda

*   <del>Icebreakers!</del>
*   Intro To Web Development
*   Coding Environment
*   HTML Basics
*   CSS Basics
*   Our First Webpage

---

## Course Updates

*   [Moodle](http:/google.com)
*   You should have gotten an email welcoming you to the class
*   I will post assignments, handouts and updates there, along with this online syllabus
*   You'll turn in your homework as zip files there

--

## What we're going to learn
(really)

*   \#1 priority is learning to find your own answers!
*   But in concrete terms, how to start a website from scratch.
*   Create semantically meaningful HTML pages
*   Style them (mostly) to your liking using CSS
*   At _least_ be able to find, understand and apply pre-written javascript interaction to your pages with aplomb!

--

## Don't expect to learn...

*   We're not doing any back-end stuff, though I are more than happy to answer specific questions.
*   That means no WordPress, Drupal, Ruby on Rails, Node, etc.

--

## Class Environment

*   Ask me lots of questions!
*   Ask each other lots of questions!
*   Let's keep it light.

---


## Intro To Web Development


---

## What is Web Development?

--

## What is Web Development?

* The practice of creating applications and experiences that users interact with via the World Wide Web.
* Most often, the act of turning ideas and design compositions into a real, usable website.
* Made up of many smaller disciplines, but primarily two...

---

## Front-End Web Development

**Client-Side**

The _client_ is the application the end-user runs to use your website.
In most cases, a web browser such as Chrome or Firefox, but there are tons of possible clients out there!

* Mobile browsers
* A [Pizza button](http://piepal.me/)
* A [Toothbrush?](http://www.npr.org/blogs/alltechconsidered/2014/01/06/260189445/ces-2014-toothbrush-bed-car-put-some-internet-on-it)
* Others?

Note:
* Mobile phone
* Screen readers for the disabled
* Scrapers (Open data, etc)
* A search bot (Crawlers for Google, Yahoo!, etc.)
* A Roku or other consumer web-enabled device

--

## The web works everywhere

And this is why it is awesome.

Note:
Front-end is all about keeping the 'everywhere' in mind, and making the best
experience possible in every context.

--

## Front-End Web Development Languages

*   HTML
*   CSS
*   JavaScript

Note:
* Each of these languages has abstractions that make them more powerful, or more like "familiar" backend languages:
  HAML, SASS, CoffeeScript.
* Some people love them, some people hate them.

---

## Back-End Web Development

**Server-Side**

The _server_ is the thing that handles the requests coming from your client. Back-end code runs only on the server, and responds in languages the client understands.

Note:
Every web page meant for public use needs a server, but that doesn't necessarily mean server-side coding.

--

## Back-End Web Development Languages

*   Ruby   ([Ruby on Rails][1], [Sinatra][2], [Padrino][3])
*   PHP    ([WordPress][4], [Drupal][5], [Laravel][6])
*   Python ([Django][7], [Flask][8])
*   PERL   ([Movable Type][9])
*   C++    ([.NET][10])
*   A bajillion others!

[1]: http://rubyonrails.org
[2]: http://sinatrarb.com
[3]: http://padrinorb.com
[4]: http://wordpress.org
[5]: http://drupal.org
[6]: http://laravel.com
[7]: http://djangoproject.com
[8]: http://flask.pocoo.org
[9]: http://movabletype.org
[10]: http://www.microsoft.com/net

--

## Do You _Need_ a Back End?

**Nope!** Some websites are _static_, meaning there's no back-end development at all - the server just responds with exactly the files that were requested.

Note:
This is where we're gonna be hanging out - you can do a lot with just front-end code, especially with all the 3rd party APIs out there nowadays.
* [Backlift](http://gun.io/blog/Building-Backbone.js-apps-with-Backlift-Views-and-Templates/)  
* [Google spreadsheets](http://www.html5rocks.com/en/tutorials/webcomponents/yeoman/)

---

## The Whole Process

From Idea to Deployment

--

## Research

*   User interviews
*   Bucketing / Themes
*   Frameworks & Synthesis
*   Brainstorming

Resource:
[IDEO's Human-Centered Design Toolkit](http://books.ideo.com/)

--

## Research Alternatives

*   Fabricated User Personas / Scenarios
*   User Surveys
*   Focus Groups

Note:
Not every budget allows for travel, pay for interviewees, tons of time spent on the ideo process

--

## UX Design / Prototyping

*   Prototypes are models of an interaction or the process to complete a task
*   Validate against user needs / scenarios
*   Low-fi vs Hi-fi
    *   Sketches on paper vs. Barebones, "fake" web pages
    *   Test in "meatspace" first
*   Iterate!

Resource: [UIE Articles Archive](http://www.uie.com/articles)

Note:
* You can prototype like playing chess: draw, interact, repeat.
* Let's try it in class (time permitting), with a FB mobile chat exercise.

--

## Information Architecture

*   How content is organized
*   Structure & Hierarchy
*   Sitemaps, Wireframes
*   Informed by lessons learned from prototype phase

Resources:

* [OmniGraffle (Mac, $50)](http://omnigroup.com/omnigraffle)
* [EightShapes Unify (InDesign)](http://unify.eightshapes.com)
* [Balsamiq (Cross-platform, $80)](http://balsamiq.com)
* [UXPin (Cloud, $15/mo)](http://uxpin.com)


--

## Visual Design

*   What it actually looks like
*   Branding, User Interface elements, Colors
*   Design systems are more flexible than one-offs

Resources:

* Laura Kalbag: [Design Systems](http://24ways.org/2012/design-systems/)
* Samantha Warren: [Style Tiles](http://styletil.es)
* Dan Mall: [Element Collages](http://danielmall.com/articles/rif-element-collages/)

* Pixelmator (Mac, $30): [pixelmator.com](http://www.pixelmator.com)
* Pixlr (Cloud, $0): [pixlr.com](http://www.pixlr.com)

--

## Front-End Development

*   Turning PSDs into \*real\* web pages
*   HTML structure, styles, JavaScript interactions

Resources:

* [Macaw](http://macaw.co)
* [Adobe Edge](http://html.adobe.com/edge/)
* This Class!

--

## Back-End Development

*   Customizing the experience to the individual user
*   User accounts, Data & payment submission, Saved data
*   Anything dealing with information that can't be sent to "everyone"

Resource: [Stack Overflow](http://stackoverflow.com)

--

## Deployment

*   Putting your code on a "production" server
*   Makes your site available to the public
*   DNS (Domain Name System) configuration maps your domain to your server
*   Can be as simple as copying files to a folder with FTP,
*   Or as complicated as a scripted process with database migrations, dependency installation, etc.

Resources:

* 90s Music  
* Hard Drugs

---

## Coding Environment

What do our computers and a web server have in common?

--

A URL

![A url](../img/unit_1/server-path.png)

--

A Finder Winow

![A finder window](../img/unit_1/file-path.png)

--

## Without a backend, the Web is just files in folders on a computer somewhere.

Note:
Let's be that somewhere!

--

We're going to create a folder called **FEWD** on your desktop, and keep all of our course work there.

--

In FEWD, add a folder called **class00**. We'll create folders in here for our coding exercises today. You can think of each folder that pertains to a specific exercise or lab as its own website. Essentially, that's what it is.

--

All of the files (HTML files, images, stylesheets, etc.) that are related to a given website should go in that site's folder, not someplace else on your computer.

--

Go to folder (in your mac's finder)

**cmd+shift+G**

--

**~** is your 'home folder'  
**~/Desktop** is your desktop,  
**~/Documents** is your documents folder, etc.

--

Start typing and hit **tab** to autocomplete!
![Tab completion in finder](../img/unit_1/tab_completion.png)

---

## Atom

![Atom](../img/unit_1/atom.png)

--

Atom is *fantastic* and is completely free

https://atom.io/

Open the .dmg file and drag the icon to your applications folder.  
Windows: Run installer(?)

--

## Opening Files in Your Browser

**Let's create our first webpage.**

1.  Make a folder inside `class00` called `hello`. Drag `hello` onto the Sublime Text icon in your dock to open it.
1.  Right-click on `hello` in the sidebar, select `New File...`.
1.  Call it index.html (Look at the bottom of the app for the text field where you name the file).
1.  Open the file and type `<h1>hello, world!</h1>`
1.  Save the file. (`cmd+s` on mac, `ctrl+s` on windows/linux)
1.  Right-click `index.html` in the Sublime sidebar and choose `Open In Browser`.

---

## The Anatomy of a URL

![URL parts](../img/unit_1/anatomy-url.png)

--

## Protocol

![URL parts](../img/unit_1/anatomy-url.png)

_**noun:** a system of rules that explain the correct conduct and procedures to be followed in formal situations_

--

Protocols govern how our computer communicates with a remote service.

--

<blockquote class="twitter-tweet" lang="en"><p>The "http://" at the beginning of URLs is a command to the browser. It stands for &quot;head to this place:&quot; followed by two laser-gun noises.</p>&mdash; Brian Sutorius (@bsuto) <a href="https://twitter.com/bsuto/statuses/172070369035956224">February 21, 2012</a></blockquote>

--

**H**yper**T**ext **T**ransfer **P**rotocol (**S**ecure)

The internet is just a way of pushing text back and forth between computers.  
HTTP is a standard for how that text is structured.

--

You can also view a webpage using 'file protocol'

`file:///Users/you/Desktop/FEWD/class00/hello/index.html`

note:
3 slashes instead of 2!?  
The extra slash tells the browser that the path starts at the root of the hard drive, not where the browser happens to live.

--

## Host (or Domain)

![URL parts](../img/unit_1/anatomy-url.png)

*   You're probably pretty familiar with these already.
*   These are mapped to IP Addresses, via something called DNS (Domain Name System).

--

## Path

![URL parts](../img/unit_1/anatomy-url.png)

*   Represents the resource on the server you're trying to access.
*   Folders are delimited by slashes.

--

## Querystring

![URL parts](../img/unit_1/anatomy-url.png)

*   A way to pass extra information not related to the 'resource' to the server.
*   Not all that relevant to static websites, generally.

--

## Hash

![URL parts](../img/unit_1/anatomy-url.png)

*   A reference to a particular spot on the page.
*   We'll learn how to create these spots later.

---

## Homework

* Watch [this video](http://www.dontfeartheinternet.com/01-not-tubes/) about the Internet.
* Read [this article](http://www.theguardian.com/help/insideguardian/2009/sep/28/blogpost) about web development.
