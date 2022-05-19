## CSS 
- Can be included in [[HTML & CSS Primer]] or written in separate stylesheet (css file)
- option 1: css style as html attribute, e.g. </a style="...">
- option 2: css style as html element, e.g. </style>...</style>
- option 3: link to style sheet located in head of html
	- head used for meta data because content not read out on website
	- optimal solution as it separates html and css and makes both easier to read


- css can be applied to element, e.g. a or h1
- css can also be applied to classes and IDs, e.g. .firstclass or #uniqueID
- css can also be applied to descendants, e.g. ".firstclass > a" will target all anchor elements nested directly inside the firstclass elements
- css can be applied to children only (i.e. not all descendants), e.g. "firstclass" will traget  target only the anchor elements that are direct children of firstclass

![[CSS specificity hierarchy.gif]]

## Pseudo classes
- used with colon, e.g. "firstclass:hover"
- examples: 
	- hover: sets values for element when mouse is hovering above 
	- focus: sets values for element focused via tab 

## Commands
- some commands are listed in [[HTML & CSS Primer]]
- line-height: can be used to create space between lines of text
- useful img attributes: aspect-ration; object-fit;

## CSS Reset
- templates online
- create separate css file, eg. reset.css
- clears all preconfigured styles so that they do not interfere with our work

## Flexbox
- [[Flexbox]]

## Google Fonts 
- lets you create customized fonts
- in css type @import url("...")
- apply font in body

## Links
- Usplash for images
- heroicons for icons as svg files
- dribble for inspiration


