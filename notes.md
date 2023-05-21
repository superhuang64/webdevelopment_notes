# Front-end Web development learning notes
intro...

-------

### Table of Contents:
sources 
pre-knowledge 
html
css
javascript

### Sources
Documentation library: MDN, W3 Schools, Dev Docs Audio

---------------------


## Pre-knowledge:
How the internet work
-   Client---ISP(internet service provider)---domain name server(DNS server)
3 types of files:
HTML(raw content), CSS(styling), JAVASCRIPT(allow action, functionality, user interection)


## Html 1                             

Introduction to HTML

### Html
-   Hypertext markup language
-   Content and structure
   - Hypertext: hypertext/hyperlinks
   - Markup language: All html5 tags()

note:
 <> tag vs element:  
 - <>:openning/closing tag 
 - Element: including content
 
### Html elements
[Html elements doc](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)


### The heading element
	• Heading tag: 
		○ h1 to h6(size)
		○ Start and end tag:<h1> content </h1>
		○ Normally one h1 in one file; don't skip the level

### The paragraph element
Distinguish between 2 paras
Lorem lpsum---get natural looking p

### The void element
<p>content</p> vs <hr />
No content in between
	• Self closing tag:
		○ <br/> or <br> break element, to a new row
		○ <hr/> or <hr> Horizontal rule element, a line: 
			§ <hr size = '3' noshade>
			§ Element + attributes

### The list element
HTML lists
	• Unordered lists+ list items:Bullet point
	<ul>
	<li></li>
	</ul>
	• ordered lists+ list items:Number 
	<ol start="5">
	<li></li>
	</ol>

### Nesting and indentation(code formatting)
Get nested list
Use indentation to check errors

### The anchor element
HTML links(additional attribute) and anchor tags
	• Link to external sites: <a href='http…'>link name</a>
	• Link to internal sites: create new html file

### The image element
Self-closing tag
<img src="url"  alt="sunset"/>
	• Size can be set
	• The Alt attribute
		○ Alt---altervative text description, screen reader
		○ Silktide extension for reading the alt
Photos Tools: 
	• circle image crops https://crop-circle.imageonline.co/
	• image editor https://www.befunky.com/create/resize-image/

### Html attributes
<tag attribute=value>content</tag>
	• Global attribute: 
		○ ex. Draggable={true}
	• Specific attribute for matching elements

## Html 2
Multi-page websites            

### Computer file paths
Absolute and relative paths
	• Absolute file paths:relative to the root
	• Relative file paths:relative to the current location

Special characrters
../essay.docx       go up a level
./essay.docx        stay in the current level(can also move the ./, but better not move)

### Html boilerplate
Html boilerplate
	• Shortcut in vs studio: !
	• .html
Good Indentation helps
Must:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    <h1>Hello World!</h1>
</body>
</html>

### Project:portefolio website

### Publish website on github
Main website: only named index.html
Web hosting:put the file to the web server
Github-repository-settings-pages-branch-select to main-get url

### Capstone projects
Show your skill through:
Personal website
Github- pinned repository/activity level

### Capstone projects- online resume


--------------------------------------------
Difference: <i><em>; <strong><bold>

HTML tables &layout
	• Table template <table><tr><th><td><thead><tbody><tfoot>
	• <table cellspacing='20'>
	• <td>column, <tr>row

Emojis 
Mac: command+control+space

HTML form
	• <form><label><input> name=''
	<form action="/action_page.php" method="get">
	        <label for="fname">First name:</label>
	        <input type="text" id="fname" name="fname"><br><br>
	        <input type="submit" value="Submit">
	      </form>
	• for creating an HTML form for user input.
	• Action: Mailto….
	• Various types can try
------------------
# Introduction to css                   

## Css 1
### Css: Cascading styling sheet
Cascading 
styling sheet language
Separate the html and style

Three types:
Inline, internal, external

### Inline css
<html style="background:blue"></html>
Style attribute(global, for all elements)
Css code: 
"property: value"
Good for single element

### Internal css
Defined in<head> section
Selector:target and select
Only target to single web page
<head>
<style>
html{
background:blue
}
</style>
</head>

### External css
Separate file
Naming: styles.css
Link the style sheet file to html
Inside the <head>, relationship and location
 <head>
<link rel="stylesheer" href="./styles.css" />
 </head>

### Css selectors
Css syntax:
Css selector{Property:value}
	• Element selector
	• Class selector#
		○ Can add as a attribute for many elements
		○ class = "red-text"
	• Id selector.
		○ Only for one element
	• Attribute selector
		○ P[draggable="false"]{color:red};
	• Universal selector
		○ *{color:red}

Css selector
	• Tag selector------ h1
	• Class selector(can be accumulated)----- .bacon circular
	• Id selector: more specific(priority to apply, only once)----- #heading
Pseudo: img:hover(touch change color)


Project-color vocab website

Css colors
{
color:(text-color)
background-color:
}
Get color:
	• <Named-color>
	• Color hunt: can customize the rgb
	Change text color css
	https://colorhunt.co/
	

Font properties
h1{font-size:20px}
1px(pixel)=1/96th inch=0.26mm
1pt(point)=1/72nd inch
1em=100% of parent size(relative size)
1rem=100% of root(more consistent way, recommend)

Font weight
h1{font-weight:bold}
Three ways to describe
Keywords:normal,bold
Relative to parent:lighter(-100),bolder(+100)
Number:100-900

Font family
h1{font-family:helvetica,sans-serif}
h1{font-family:"Times New Roman",sans-serif}
Get font:
Google fonts
	• https://fonts.google.com/
	• Copy the link to <head>section

Text align
h1{text-align:center}
Start,end,justify
Put text/image in the center
Body{text-align: center}
	• If width:10%, not in the conter
	• Add auto margin
	• Margin: 0 auto 0 auto


Css inspection
Chrome devtool(command+option+I)
Computing
More tools-css overview

The css box model-margin,padding and border
Content-padding-border-margin
Extension: pesticide---highlight all boxes
border:10px solid black;
     border-top:0px;
     border-width:0px 10px 20px 30px;(top right bottom left)
     border-width:0px 20px;((top bottom )(right left ))
Padding:20px;
	• Push border out by 20px(between the element and the border)
Margin:
	• Outside the border
	• Make the two boxes touch edge to edge: calculate the margin
	• Order: top, right, bottom, left
	• Value: auto(can make the position re-center when change the width ), length, %, inherit
	• Don't have to always type all values--check the rule

Content division element
Wrap into one same box-<div>
	• <div></div>
Can be visible via css styles or content(inside div)
Default value for body: have margins
How to check and change the format
	• Tool: pesticide+ google inspect---test

Project- motivational poster website

The cascade- specificity and inheritance
	• Position  lower being written, more important
	• Specificity: id>attribute>class>element selector
	• Type:inline>internal>external
	• Importance: 
	color:green !important;

Combining css selectors
Group selector
	• h1,h2{}
Child selector
	• Selector > direct child selector{}
	• .box > p
Descendent selector
	• matches all elements that are descendants of a specified element.
	• Selector Selector {}
	• div p {
	  background-color: yellow;
	}
Chaining selector
• SelectorSelector {}
Apply where all selectors are true
Start with the element
Combining selector
• Selector SelectorSelector {}

Css positioning
{position: value}
	• Property:position
	• Four values: Static relative absolute fixed
	• Seperate from margin
	• {position:static;
	Top:20px
	Left:
	Bottom:
	Right:
	}
Position(property)
	1. Static: html default flow
	2. Relative: 
	• Relative to itself based on the values
	• Other elements won't be affected
	• Coordinate: top, bottom, left, right
	• {Position:relative 
	Top:-200px
	Left:20px}
	3. Absolute
	• Removed from current document flow
	• Relative to the nearest positioned parent ancestor or top left corner of the web page 
	• Affect Other elements' positions 
	• .container: used to nest sth in to create another parent box
	4. Fixed
	• Relative to top left corner of the browser window
	• When scroll the page, it still fix in the page position

Border-radius:50%
Perfect circle

Project----css flag

Css display
 h2{display:block}
Block display
	• the whole width display- full width block
	• Can set size
	• Another element will go below it 
	• Common block elements:<p><h1><div><ol><form>…
Inline display element
	• within the line, can set elements go on in the same line
	• next can add as long as there's space
	• Default to their size of content, can't change the width and height
	• <span><img><a>(anchors)
Inline-block display
	• Set the size& go on in the same line
	• <p> <style>:display=inline-block
None display
	• Make the element disappear and no position
	• P{display:none}
	• P{visibility:hidden}---keep blank position

Css float--float and clear
Wraping text using float and clear
<img …/>
<text>text</text>
<footer>copyright</footer>
Img{
Float:right
}
Footer{
Clear:left
}
Float(position)
	• Float: left/right
	• Put the image(or other element) in the left side of the text
	• Only used in cases of wrapping text, recommend for wrap text and image
	.photography {
	    width: 25%;
	    float: right;
	    margin: 30px;
	}
Clear
	• Clear some position, put part of the text under the image
	• The element is cleared of the left float
/*.computer-description {
    clear: left
}*/
