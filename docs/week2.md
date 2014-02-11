% HTML & CSS

Document Structure
------------------------

* [labor1.html](web/labor1.html) [code](https://github.com/mcuringa/teaching-labor/blob/master/web/labor1.html)
  uses basic html structures to format the page
* header tags: ``h1, h2, h3, h4``
* paragraph tag: ``p``
* bold and italic: ``strong``, ``em`` (emphasis)
* un-ordered list: ``ul``, ``li``

Declaring an html document
-----------------------------

~~~~~~~~~~~~~~~~~~~~~~~~~~~{.html}
<!DOCTYPE html>
<html>
    <head>
        <title>Teaching Labor, an Adelphi University MOOC</title>
    </head>

    <body>
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Links
=============

Hyper Links
---------------------------

* links make the Web what it his
* HTML --> hyper text markup language
    * not the first/only type of hypertext
    * allows documents on different computers to link to each other
* thinks we link to:
    - other web pages
    - images (photos, etc)
    - video
    - audio
    - javascript resources
    - cascading stylesheets (css)

URL Basics
--------------------------

![](http://media.creativebloq.futurecdn.net/sites/creativebloq.com/files/images/2012/01/NET215_tut_url_diagram_615x246.jpg)

* _via_: <http://www.creativebloq.com/design/design-perfect-url-1126509>

Absolute URLs
------------------
* **absolute urls**: link to an external site

~~~~~~~~~~~~~~~~~~~~~~~~~~~{.html}
<a href="http://matt.curinga.com">click here</a>
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Relative URLs
------------------
* **relative urls**: link to a resource on the same website

~~~~~~~~~~~~~~~~~~~~~~~~~~~{.html}
<strong>Navigation</strong>
<ul>
  <li><a href="home.html">Home</li>
  <li><a href="news.html">News</li>
  <li><a href="about.html">About</li>
</ul>
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Relative from root
--------------------
* URLs starting with a  forward slash (``/``) start from the root of the website
* this allows developers to link to resources without having to know where it is
  relative to the linking page
* makes it easier to **reuse** code snippets on multiple pages

~~~~~~~~~~~~~~~~~~~~~~~~~~~{.html}
<strong>Navigation</strong>
<ul>
  <li><a href="/home.html">Home</li>
  <li><a href="/news.html">News</li>
  <li><a href="/about.html">About</li>
  <li><a href="/about/matt.html">About</li>
  <li><a href="/about/hannah.html">About</li>
</ul>
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Internal links
---------------------
* can be used to "jump" to a section of a page
* you can declare anchors (jump targets) by using the ``id`` attribute on an html element
* the link starts with the ``#`` sign

~~~~~~~~~~~~~~~~~~~~~~~~~~~{.html}
<a href="http://en.wikipedia.org/wiki/Hypertext#History">Go to Wikipedia 
HyperText article and jump to the history section</a>
~~~~~~~~~~~~~~~~~~~~~~~~~~~

~~~~~~~~~~~~~~~~~~~~~~~~~~~{.html}
<!-- from wikipedia page -->
<h2 id="history">History</h2>
<p><a href="/wiki/Hypertext" title="Hypertext">Hypertext</a> (...)</p>
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Title attribute
---------------------

* ``a`` tags have an optional ``title`` attribute
* the title gives more information to the user before they click a link
* it's often in the form of a tool tip
* titles also provide additional semantic information about a page

~~~~~~~~~~~~~~~~~~~~~~~~~~~{.html}
<a href="http://matt.curinga.com"
   title="check out my home page">click here</a>
~~~~~~~~~~~~~~~~~~~~~~~~~~~



Link to a stylesheet
-------------------------

* a stylesheet on the same webs server, _relative link_

~~~~~~~~~~~~~~~~~~~~~~~~~~~{.html}
<link href="css/labor3.css" type="text/css" rel="stylesheet" />
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
