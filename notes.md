# Front-end Web development learning notes
This is my learning notes relating to web developent. 

---

### Table of Contents:
- Sources 
- Intro to front-end web development 
- Html
- Css
- Javascript

### Sources
Documentation library: 
MDN, W3 Schools, Dev Docs Audio

get natural looking paras:
[Lorem lpsum](https://loremipsum.io/)

image Tools: 
- circle image crops https://crop-circle.imageonline.co/
- image editor https://www.befunky.com/create/resize-image/

Codeply: https://www.codeply.com/
 allows to include the framework of bootstrap

### shortcuts/tool
Emojis 
Mac: command+control+space

css overview inspection
Chrome devtool(command+option+I)
Computing
More tools-css overview

Extension: pesticide---highlight all boxes
---

## Intro to front-end web development 
How the internet work
- Client---ISP(internet service provider)---domain name server(DNS server)
3 types of files:
- HTML(raw content)
- CSS(styling)
- JAVASCRIPT(allow action,functionality, user interection)

## Html 1-Introduction to HTML
- what is HTML?
- HTML elements:heading,paragraph,void,list,anchor,image
- concept: HTML tag, HTML elements, HTML attribute
- Nesting and indentation
---
### Html
- Hypertext markup language
- Content and structure
  - Hypertext:hypertext/hyperlinks 
  - Markup language: All html5 tags()  

note:
 tag vs element:  
 - `<tag></tag>`:openning/closing tag 
 - Element: including content
 
### Html elements
[Html elements doc](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

**The heading element**
Heading tag: 
- h1 to h6(size)
- Start and end tag:`<h1> content </h1>`
- Normally one h1 in one file; don't skip the level

**The paragraph element**
`<p></p>`:Distinguish 2 paras
get natural looking p:
[Lorem lpsum](https://loremipsum.io/)

**The void element**
no child nodes--No content in between,self closing tag
- `<br/>` or `<br>`:break element, to a new row
- `<hr/>` or `<hr>`:Horizontal rule element, a line
  - `<hr size = '3' noshade>`
  - Element + attributes

**The list element**
HTML lists
- Unordered lists + list items:Bullet point
	```
	<ul>
	<li></li>
	</ul>
	```
- ordered lists + list items:Number 
	```
	<ol start="5">
	<li></li>
	</ol>
	```

**Nesting and indentation(code formatting)**
Get nested list
Use indentation to check errors

**The anchor element**
HTML links(additional attribute) and anchor tags
- Link to external sites: `<a href='http…'>link name</a>`
- Link to internal sites: create new html file

**The image element**
Self-closing tag
`<img src="url"  alt="sunset"/>`
- Size can be set
- The Alt attribute
  - Alt---altervative text description, screen reader
  - Silktide extension for reading the alt
image Tools: 
- [circle image crops](https://crop-circle.imageonline.co/)
- [image editor](https://www.befunky.com/create/resize-image/)

### Html attributes
`<tag attribute=value>content</tag>`
- Global attribute: 
  - ex. `draggable={true}`
- Specific attribute for corresponding elements

---
## Html 2--Multipage websites            
- what is Computer file paths,how to use it?
- Html boilerplate
---

**Computer file paths**
Absolute and relative paths
- Absolute file paths:relative to the root
- Relative file paths:relative to the current location

Special characrters
`../essay.docx `   go up a level
`./essay.docx`     stay in the current level(can also move the ./, but better not move)

**Html boilerplate**
Html boilerplate
- Shortcut in vs studio: !
- extension: .html
Good Indentation helps
Musboilerplate:
```
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
```

**Project:portefolio website**

**Publish website on github**
Web hosting:put the file to the web server
Main website page: only named index.html
steps:Github-repository-settings-pages-branch-select to main-get url

**Capstone projects**
Show your skill through:
Personal website
Github- pinned repository/activity level

**Capstone projects- online resume**


---
haven't organised 

Difference: <i><em>; <strong><bold>

HTML tables &layout
	• Table template <table><tr><th><td><thead><tbody><tfoot>
	• <table cellspacing='20'>
	• <td>column, <tr>row



HTML form
	• <form><label><input> name=''
	<form action="/action_page.php" method="get">
	        <label for="fname">First name:</label>
	        <input type="text" id="fname" name="fname"><br><br>
	        <input type="submit" value="Submit">
	      </form>
	• for creating an HTML form for user input.
	• Various types can try
---
# Introduction to css                   

## Css 1

### Css: Cascading styling sheet
css: Cascading styling sheet language
Separate the html and style code
Three types:
- Inline, internal, external

**Inline css**
`<html style="background:blue"></html>`
`style` attribute---global, for all elements
Css code: "property: value"
Good for single element

**Internal css**
Defined in`<head>`section
Selector:target and select
Only target to single web page
```
<head>
<style>
html{
background:blue
}
</style>
</head>
```

**External css**
Separate file
Naming: styles.css
Link the style sheet file to html
Inside the <head>, relationship and location
 <head>
<link rel="stylesheer" href="./styles.css" />
 </head>

### Css selectors/significance/combine

1. selectors
Css syntax:
Css selector{Property:value}
- Element selector
- Class selector #
  - `class = "red-text"`
  - can add as an attribute for many elements
  - can be accumulated----- `.bacon .circular{}`
- Id selector .
  - Only for one element----- #heading
  - priority to apply
- Attribute selector
  - `p[draggable="false"]{color:red};`
- Universal selector
  - `*{color:red}`
Pseudo: 
`img:hover{};`(touch change color)

2. importance order
The cascade- specificity and inheritance
- Position:lower being written, more important
- Specificity: id>attribute>class>element selector
- Type:inline>internal>external
- Importance: `color:green !important;`

3. Combining css selectors
- Group selector:`h1,h2{}`
- Child selector:
  - select all the child elements inside the parent
  - `Selector > direct child selector{}`
  - `.box > p`
- Descendent selector
  - matches all elements that are descendants of a specified element.
  - `Selector Selector {}`
```
div p {
	  background-color: yellow;
	}
```
- Chaining selector
  - `SelectorSelector {}`
  - Apply where all selectors are true
  - Start with the element
- Combining selector
  - `Selector SelectorSelector {}`

---

**Project-color vocab website**

---

## css properties

**Css colors properties**
```
{
color:(text-color)
background-color:
}
```
Get color:
- Named-color in doc
- [Color hunt](https://colorhunt.co/): can customize the rgb

**Font properties**
1. font size
`h1{font-size:20px}`
1px(pixel)=1/96th inch=0.26mm
1pt(point)=1/72nd inch
1em=100% of parent size(relative size)
1rem=100% of root(more consistent way, recommend)

2. Font weight
`h1{font-weight:bold}`
Three ways to describe
Keywords:normal,bold
Relative to parent:lighter(-100),bolder(+100)
Number:100-900

3. Font family
`h1{font-family:helvetica,sans-serif}`
`h1{font-family:"Times New Roman",sans-serif}`
Get font:
[Google fonts](https://fonts.google.com/)
- Copy the link to`<head>`section

**Text align**
`h1{text-align:center}`
Body{text-align: center}
- put text/image in the center
- value:start,end,justify
dev tool-css overview-check the css properties

**The css box model-margin,padding and border**
box:Content-padding-border-margin
Extension: pesticide---highlight all boxes
1. border
```
border:10px solid black;
     border-top:0px;
     border-width:0px 10px 20px 30px;(top right bottom left)
     border-width:0px 20px;((top bottom )(right left ))
```
2. padding 
`Padding:20px;`
- Push border out by 20px(between the element and the border)
3. Margin
`margin:0 auto 0 auto; `
- Make the two boxes touch edge to edge: calculate the margin
- Order: top, right, bottom, left
- Value: auto(can make the position re-center when change the width ), length, %, inherit


**Content division element**
`<div></div>` 
Wrap into one same box for organizing styling
Can be visible via css styles or content(inside div)
Default value for body: have margins
How to check and change the format
- Tool: pesticide+ google inspect---test

**Project- motivational poster website**

### Css positioning
`{position: value}`
- position as property
- Seperate from margin
- Four values: Static relative absolute fixed
```
{position:static;
	Top:20px
	Left:
	Bottom:
	Right:
	}
```
1. Static: html default flow
2. Relative: 
  - Relative to itself based on the values
  - Other elements won't be affected
  - Coordinate: top, bottom, left, right
	```
	{Position:relative 
	Top:-200px
	Left:20px}
	```
3. Absolute
  - Removed from current document flow
  - Relative to the **nearest positioned parent ancestor or top left corner** of the web page 
  - Affect Other elements' positions 
  - `.container`: used to nest sth in to create another parent box
4. Fixed
  - Relative to top left corner of the browser window
  - When scroll the page, it still fix in the page position

---
Border-radius:50%
Perfect circle

Project----css flag

---
### Css display
**Block display**
- h2{display:block}
- the whole width display- full width block,Another element will go below it 
- Can set size
- Common block elements:`<p><h1><div><ol><form>`…
**Inline display element**
- within the line, can set elements go on in the same line
- next can add as long as there's space
- Default to their size of content, can't change the width and height
- `<span><img><a>`(anchors)
**Inline-block display**
- Set the size& go on in the same line
- `<p> <style>`
**None display**
- Make the element disappear and no position
- `P{display:none}`
- `P{visibility:hidden}`---keep blank position

### Css float--float and clear
Wraping text using float and clear
```
<img …/>
<text>text</text>
<footer>copyright</footer>
```
```
Img{
Float:right
}
Footer{
Clear:left
}
```
**Float**(position)
- Float: left/right
- Put the image(or other element) in the left side of the text
- Only used in cases of wrapping text, recommend for wrap text and image
	.photography {
	    width: 25%;
	    float: right;
	    margin: 30px;
	}
**Clear**
- Clear some position, put part of the text under the image
- The element is cleared of the left float
```
.computer-description {
    clear: left
}
```
## Build responsive website
Respond to the change of screen size
Four ways:
- Media queries
- Css grid
- Css flexbox
- External framework ex.bootstrap

### Media query 
[Doc](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)
**Media type**
```
@media screen, print {
  /* … */
}
```
**Media feature**
Adding breakpoints to define responsive layouts
	• Mobile-first
	• Mobile-friendly test
	• Make a separate mobile site/make it responsive(css native function)
Factors of Size:
	• Device, browser, viewer
	• Decide the border of the size to change
`@media(type and type and type){feature}`
- Combine multiple features:
```
@media(max-width:1028px) and (min-width:702px){
H1{font-size:15px}}
```

**Project- Web design agency website**

### Flexbox
Don't use table, float for layout
Steps:
- Wrap the content in a container
- Set the container display to flex
- Set the gap

Default display value
`<div></div>` block
`<span></span>` inline
Can use flex box container to include all of them, and ignore the inner display setting(block,inline-block, inline)
The width of each element is depend on the content
Display:inline-flex

**Flex direction**
`Flex-direction:row/column`
From top to bottom
From left to right 
Flex-basis
Height/weight
Flexing along the main axis
.container{
Display: flex;
Flex-direction:column;
}
Select all the children inside the container
.container > *{
Flex-basis:100px;
}

Flexible layout
Align, justify and wrap
Row and column layouts
Figure out the property is for child or parent selector

For child elements
Rearrange the order of the child elements
Set the order property
Default: order:0---the order by the html
.green{order:2}---in the end
.green{Align-self:center;
height:80px}

For parent container
Flex-wrap:nowrap;---default
Flex-wrap:wrap;-----fit its full width,go to next line
Justify-content:flex-end/flex-start/center
When there's space left, push all to the right/left/center
Justify-content:space-between/space-around/space-evenly
create space between each child elment
Align-content(when wrap)
Align-items:start;(when unwrap)
Height:80px;----the viewport height

game:
flexbox-froggy

Guide to flexbox
https://css-tricks.com/snippets/css/a-guide-to-flexbox/

Flex-sizing
Shrinking and growing
Priority list:
Max-width/min-width> flex-basis>width>content width(word,sentence)

Default content width
Max-width:longest sentence
Min-width:longest word

Flexitems:
Default-----
Flex-basis:100px;
Flex-grow:0;
Flex-shrink:1;

Flex-basis:auto;---default, based on the content
Flex:1;-------grow1,shrink1,basis0

Box Ratio:1:2:3
Flex:1;
Flex:2;
Flex:3

Project-prizing table

Css grid 
A two-dimensional layout system
Flexbox( one dimensional layout)
Most, Combination of flex and grid
<div class="container">
<p>…</p>
<p>…</p>
<p>…</p>
<p>…</p>
</div>

.container{
Display:grid;
Grid-template-columns: 1fr 2fr;
Grid-template-columns:1fr 1fr;
Gap:10px;
}

Grid sizing 
Size columns and rows
Not responsive
.container{
Display:grid;
Grid-template-columns: 100px 200px;
Grid-template-columns:400px 800px;
}
Simplied version
.container{
Display:grid;
Grid-template: 100px 200px/400px 800px;
}
Responsive
Auto---
.container{
Display:grid;
Grid-template-columns: 100px auto;---fit the content
Grid-template-columns:400px auto;---fit the row
}
Fraction size
.container{
Display:grid;
Grid-template-columns: 1fr,2fr;
Grid-template-columns:1fr,2fr;
}
Minmax size grid 
.container{
Display:grid;
Grid-template-columns: 100px 200px
Grid-template-columns:200px minmax(400px,800px)
}
Repeat grid
.container{
Display:grid;
Grid-template-columns: repeat(2, 200px);----200px 200px
Grid-template-columns:repeat(3 , 100px);---100px 100px
2*3=6 columns have been set
If only 4 exist, apply from left to right,top to bottom
If defined columns not enough,a uto match
Grid-auto-rows:300px

Use dev tools to inspect and debug it

Grid placement
Components:
Div---called grid container
Row and column tracks
Grid cell--the smallest unit of the grid
Grid lines
Items 
 flexbox work alongside grid  

Grid-column:span 2
Grid-column-start
Grid-column-end
Order:1;-----relative--put in the end if others are all default 0

Project- mondrian painting

Bootstrap 
External Css framework
Website https://blog.getbootstrap.com/
Github https://github.com/twbs/bootstrap
	• Responsive: Laptop,ipad,iphone
	• Pre-built components and styling
	• Defined class

Install bootstrap framework onto my website
	• Three ways: link/download css file/paste all template

Include CDN(Content delivery network)
Add link to <head>
Add script just before the end of <body>
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe" crossorigin="anonymous"></script>

Bootstrap container
Most commonly used two
.container
.container-fluid

Different container size based on the screen size
	• Responsive automatically
	• Class='container-fluid': 100%width

Sized columns
Add the prebuilt css classes
<div class="col-2" 

Bootstrap breakpoints
Defined based on common screen sizes
Sm-md-lg-xl------------Mobile-ipad-laptop-desktop

Multiple breakpoints
Grid system:
More Responsive
	• Div Class="row"
	• Div Class="Col-lg-3 col-md-4"
	• Default:12/100%

Dev tool
Toggle device tool bar
Check the dimension in the responsive mode
To know which breakpoint should choose

Bootstrap components
Bootstrap Button 
<button class="btn btn-primary">

Bootstrap carousel
Srcoll through different pages of images

Bootstrap cards

Bootstrap navs
Codeply: https://www.codeply.com/
	•  allows to include the framework of bootstrap

Bootstrap example+dev tool----copy elment---get the code 
Including the code from the extended css file---check it by inspect---ex. Feature.css--enter the file

Snippets 

Spacing 
Classes are named:
property-sides-size
Ex. Class="mb-2"

Dark mode
<html lang="en" data-bs-theme="dark">

Get good template
W3 school bootstrap template
https://www.w3schools.com/bootstrap/bootstrap_templates.asp

Search for free bootstrap templates
Wireframing
	• Low fidelity
	• Mock-up: high fidelity
	• UI patterns  https://ui-patterns.com/
	Sneakpeekit
	Balsamiq
Design portfolio https://ui-patterns.com/

