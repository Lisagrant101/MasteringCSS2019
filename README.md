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
