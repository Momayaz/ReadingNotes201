# How we manage the code content to creat a correct and perfect code.
* HTML pages are text documents.
* X HTML uses tags (characters that sit inside angled
* brackets) to give the information they surround special
meaning.
* X Tags are often referred to as elements.
* X Tags usually come in pairs. The opening tag denotes
the start of a piece of content; the closing tag denotes
the end.
* X Opening tags can carry attributes, which tell us more
about the content of that element.
* X Attributes require a name and a value.
* X To learn HTML you need to know what tags are
available for you to use, what they do, and where they
can go.
## Adding HTML5 Audio to Your Pages
<audiosrc="audio/test-audio.ogg"
 controls autoplay>
 to give <audio src="audio/test-audio.ogg"
 controls autoplay>
 * Flash allows you to add animations, video and audio to
the web.
* Flash is not supported on iPhone or iPad.
* HTML5 introduces new <video> and <audio>
elements for adding video and audio to web pages, but
these are only supported in the latest browsers.
* Browsers that support the HTML5 elements do not
all support the same video and audio formats, so you
need to supply your files in different formats to ensure
that everyone can see/hear them.
## CSS Associates Style rules with HTML elements

 Using Internal CSS
You can also include CSS rules
within an HTML page by placing
them inside a <styl e> element,
which usually sits inside the
<head > element of the page.
The < style > element should use
the type attribute to indicate
that the styles are specified in
CSS. The value should be text/
css.
When building a site with more
than one page, you should use
an external CSS style sheet. This:
● Allows all pages to use the
same style rules (rather than
repeating them in each page).
● Keeps the content separate
from how the page looks.
● Means you can change the
styles used across all pages
by altering just one file
(rather than each individual
page).
 * CSS treats each HTML element as if it appears inside
its own box and uses rules to indicate how that
element should look.
* Rules are made up of selectors (that specify the
elements the rule applies to) and declarations (that
indicate what these elements should look like).
* Different types of selectors allow you to target your
rules at different elements.
* Declarations are made up of two parts: the properties
of the element that you want to change, and the values
of those properties. For example, the font-family
property sets the choice of font, and the value arial
specifies Arial as the preferred typeface.
* CSS rules usually appear in a separate document,
although they may appear within an HTML page.

* Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker.
Understanding Color
Computer monitors are made
up of thousands of tiny squares
called pixels (if you look very
closely at your monitor you
should be able to see them).
When the screen is not turned
on, it's black because it's not
emitting any light. When it's
on, each pixel can be a different
color, creating a picture.
The color of every pixel on the
screen is expressed in terms of
a mix of red, green, and blue —
just like on a television screen.

* Superscript &
Subscrip
<sup >
The <su p> element is used
to contain characters that
should be superscript such
as the suffixes of dates or
mathematical concepts like
raising a number to a power such
as 22
.
<su b>
The <su b> element is used to
contain characters that should
be subscript. It is commonly
used with foot notes or chemical
formulas such as H2
* <b r />
As you have already seen, the
browser will automatically show
each new paragraph or heading
on a new line. But if you wanted
to add a line break inside the
middle of a paragraph you can
use the line break tag <b r />.
* <h r />
To create a break between
themes — such as a change of
topic in a book or a new scene
in a play — you can add a
horizontal rule between sections
using the <h r /> tag.
* <str ong>
The use of the <st rong>
element indicates that its
content has strong importance.
For example, the words
contained in this element might
be said with strong emphasis.
By default, browsers will show
the contents of a <stro ng>
element in bold.
* <e m>
The <e m> element indicates
emphasis that subtly changes
the meaning of a sentence.
By default browsers will show
the contents of an <e m> element
in italic.
* <bloc kquote>
The <bloc kquote> element is
used for longer quotes that take
up an entire paragraph. Note
how the < p> element is still
used inside the <block quote>
element.
Browsers tend to indent the
contents of the <block quote>
element, however you should not
use this element just to indent a
piece of text — rather you should
achieve this effect using CSS. 
* <q >
The < q> element is used for
shorter quotes that sit within
a paragraph. Browsers are
supposed to put quotes around
the <q > element, however
Internet Explorer does not —
therefore many people avoid
using the <q > element.
* The <tabl e> element is used to add tables to a web
page.
* A table is drawn out row by row. Each row is created
with the <tr > element.
* Inside each row there are a number of cells
represented by the < td> element (or < th> if it is a
header).
* You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.
* For long tables you can split the table into a <th ead>,
<t body>, and <tf oot>.
<in put>
type="password"
When the type attribute has
a value of password it creates
a text box that acts just like a
single-line text input, except
the characters are blocked out.
They are hidden in this way so
that if someone is looking over
the user's shoulder, they cannot
see sensitive data such as
passwords.
________________
JQUERY
The examples in this chapter revisit the list application used in the previous two chapters, and they will use jQuery to update the content of the page. ```<script src="j s/ jquery-1 .11. 0 .js "></script>```

WHY USE JQUERY?
jQuery doesn't do anything you cannot achieve with pure JavaScript. It is just a JavaScript file but estimates show it has been used on over a quarter of the sites on the web, because it makes coding simpler.

jQuery's motto is "Write less, do more," because it allows you to achieve the same goals but in fewer lines of code than you would need to write with plain JavaScript.

FINDING ELEMENTS
Using jQuery, you usually select elements using CSS-style selectors. It also offers some extra selectors, noted below with a 'jQ'.

LOOPING :
In plain JavaScript, if you wanted to do the same thing to several elements, you would need to write code to loop through all of the elements you selected. $('l i em') .addClass('seasonal ') ; $( ' li .hot') .addClass('favorite');

CHAINING
$( 'l i [i d!="one"] ') . hide() .delay(SOO) . fadeln(1400); If you want to use more than one jQuery method on the same selection of elements, you can list several methods at a time using dot notation to separate each one, as shown below

GETTING ELEMENT CONTENT
The â€¢ htm 1 () and â€¢ text () methods both retrieve and update the content of elements. This page will focus on how to retrieve element content. To learn how to update element content.

GETTING AT CONTENT
On this page you can see variations on how the . html() and . text() methods are used on the same list (depending on whether ```<ul >```or ```<li>``` elements are used in the selector). var $listHTML = ${'ul') . html(}; $ ( 'ul '). append($1 i stHTML);

UPDATING ELEMENTS
Here are four methods that update the content of all elements in a jQuery selection .

BASIC EFFECTS
In this example, it appears as if list items are faded into view when the page loads. Each item is faded out when it is clicked on.
```
 $(function() { $('h2').hide().slideDown(); var $li = $('li'); $li.hide().each{function(index) { 2 $(this).delay(700 * index) .fadeln(?OO); } ) ; 3 $li.on('click', function() $(this) .fade0ut(700); } ) ; } ) ;
```

ANIMATING CSS
The .animate() method allows you to create some of your own effects and animations by changing CSS properties.
```
$(function() { $(' l i').on( 'click', function() { ~ $(this).animate({ ~r opacity : 0.0, ~ paddingleft: '+=80' @ } , 500, function() { ~ $(this).remove(); } ) ; } ) ; } ) ;
```

All list items are selected and, when a user clicks on one of them, an anonymous function runs. Inside it, $(this) creates a new jQuery object holding the element the user clicked on. The .animate() method is then called on that jQuery object.

TRAVERSING THE DOM
When you have made a jQuery selection, you can use these methods to access other element nodes relative to the initial selection.

6 Reasons for Pair Programming
Iterative loops. Code reviews. Fast feedback. Error checking and linting. These are software engineering practices that have proven to dramatically improve the quality of code developers produce. What if you can could get all of this, instantaneously, while typing code line by line and character by character? You can, with pair programming, a technique common to many agile work environments.

How does pair programming work?
While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the â€œmechanicsâ€� of coding, the Driver manages the text editor, switching files, version control, andâ€”of course writingâ€”code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

Why pair program?
While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful

Greater efficiency
Engaged collaboration
Learning from fellow students
Social skills
Job interview readiness
Work environment readiness.
_____
