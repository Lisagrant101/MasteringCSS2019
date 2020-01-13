# MasteringCSS2019
CSS course for frameworkTV

Notes from the course
--------------------------------lesson two------------------------------------------------

STYLING TEXT
rule:
color

text-align

text-decoration

text-transform

text-indent

letter-spacing

line-height

word spacing

more detail:

Color : define with color names, rgb or hex values

Text Align : right, left, justify, center

Text Decoration : underline, overline, strikethrough

Text Transform : uppercase, lowercase

Text Identation : indents first line by X pixels.

Letter Spacing : how far apart letters are 

Line height : spaces height of letters 

Word Spacing : the width of a space between words.

Text Shadow: horizontal offset, vertical offset, color (ie 2px 2px blue).


STYLING FONT

rules

font-family

font-style

font-weight

font-size

more detail:

font-family : stick to standard common fonts

font-style : italic, normal

font-weight : number 100 to 900 or word like bold

------------------------------------------------------------------lesson 3


SELECTORS

tags : h1 , h2, p, etc

ID and Class selectors: use # and . respectively then the name of id/class.

multiple selectors : on one line with comma between.

descendant selector : [main element tag] followed by [descending tag] no comma
ie. p h2{} selects all h2 headings inside paragraphs

Descendant selector : [parent tag] > [child tag] ie. #main > h2

Attribute selector : [attribute =value]{}
use square brackets here in definition

Psuedo selector : p::first-line or p:first-letter selects only a portion of hte paragraph listed.

-------------------------------------------------------------------lesson 4
FORMS styling

form itself : width, border, padding, background color

input : width, height, margin, font-size, background color, borders (none or on bottom)

dropdone (select) : width, font-size, background color, 

*** width 100%, large font and line height, and border none are mobile friendly 

input[type=checkbox] :width, height and zoom

form p : font family, font - size

button: big height, big font, urgency color, rounded corners.

--------------------------------------------------------------------lesson 6
CSS POSITIONING

STATIC - elements line up one on top of each other, this is the default for div 'boxes'

RELATIVE - you write ie. top:300px left:100px places box at (100, 300) point relative to its default position.

ABSOLUTE - write ie. bottom:0px right 0px; puts it exactly at the bottom right corner of screen. it stays where you put it even when you 
scroll the screen.

FIXED - LIKE ABSOLUTE BUT MOVES WITH YOU WHEN SCROLLING

RESPONSIVE DESIGN

SMALL SCREENS  at a glance info

LARGE SCREENS comprehensive information

Coding: 
<meta name="veiwport" content="width=device-width, initial-scale=1"/>

<link href="reset.css" type="stylesheet"/>
You can get reset.css from eric meyer website.

Put a logical division around everything.
(css, margin padding =0)

Put a header section
(css text align center, background to grey light, width 100%, padding and border)

Put a section for all the content stories
You can put each story in the section under divs with the same class names.
(css margin and borders, border radius padding background color and box shadow, set width of individual story divs relative to whole story section)

Put a footer at the bottom
(css text align, center, border top, bottom position, width 100%, height, margin top)

(images css: width 100%)

(css: @media screen and (min-width:600px){
	change header font size to less
	change story width to half and float to left
	change story img to 50% width, float right and padding
}//this css for tablet
other formats of screens:
1024px = for desktop
default css for mobile.
Order the CSS styles : mobile> tablet> desktop.

TRANSITIONS AND ANIMATIONS
HTML->
---use reset.css for defaults
---container div for everything
---container div for content you want transitions/animations
css->
---use opacity property for selectors you will style (
---use transition property, and transform property on content selectors using the hover property.
ie. #div4Content img:hover{
transtion:opacity 1s; //
transition-delay:.25s;
transform:rotate(5deg);
transform:scale(2, 2); //2 stands for 200%
}

SPRITE SHEETS
div for background, div for moving object
audio tag set to autoplay
iframe tag to allow playing music

Back CSS-----------
	set background-image to your background
	width to 100%
	height:1022px
	z-index to -1 (higher numbers are on top of lower numbers, zindex is position of images on screen)
	animation: back 30s  infinite;
	animation-time-function:linear (means the the acceleration or deceleration of moving images can be set to ease-in or ease-out also)
@keyframes back CSS-----------
	100% {
	   set background-positon:-3027px 0; 
(-3027px moves the image to the left  by 3027 px which should be the image width for a full screen image, 0 means no yaxis movement)
sprite div CSS----------------
	uses a multiple frame repeated animation
	postion set for top and left
	width and height set to div width and height
	background-image set to url(image name)
	animation: .6s steps(6) infinite; means that there are 6 images/frames in the whole image 
	z-index:1;
	background-position:-1536px 0;
	(sets the image to move to the left the entire width of the sprite image but because the sprite div is 1/6 of the width of the background image then it bounces along the screen showing 1/6 of the image at the time)	
sound set in html

