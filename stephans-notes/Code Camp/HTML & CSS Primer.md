# HTML 
Markup language similar to but more powerful than [[Markdown]]. Almost all elements have an opening and closing tag and can be easily nested inside one another (thus called parent and children).

## Mindmap 
<iframe width="768" height="432" src="https://miro.com/app/live-embed/uXjVO1vnw5c=/?moveToViewport=-1215,-331,1864,915" frameBorder="0" scrolling="no" allowFullScreen></iframe>
## Basic Structure
- Root of website commonly called index.html
- Web servers typically look for index file as first page
- requires core code that can be auto-completed in [[Visual Code Editor]] using !Emmet
- core code:
	- !Doctype hmtl
	- html
	- head
	- body

## Box Model
- elements typically follow box-model
- boxes can be modified using style attributes: height, weight, padding, border, margin, left, right, top, bottom, display, position
	- positions:
		- "relative" moves element relative to parent element
		- "absolute" moves element relative to whole website AND removes element from flow, i.e. it does no longer move relative to other elements and may overlap 
		- "fixed" also removes it from flow and fix it relative to viewport (e.g. screen) so that it remains in place even while scrolling through page
- only boxes have padding, margin, border
- hence if we want to use and modify these values we have to use boxes
- hence the option to choose inline-boxes in display element

## Syntax
All tags need to follow: 
>>  <p>text</p> #to-do 
- the exception being <br />

- h1 to h6 -> headlines
- p -> paragraph
- ul -> unordered list
- ol -> ordered list
- li -> list items
- div -> generic container to nest other items inside; by default displays as block
- span -> normally used inside p tags to add additional styling; by default displays as inline
- strong -> changes font weight to bold
- em -> italicize text
- a -> links to page indicated in attribute href
- img -> self-contained tag for images; attributes src and alt
- svg

Full(er) List can be found at [MDN](https://developer.mozilla.org/de/docs/Web/HTML/Element)

### Table
Tables require a nested hierarchy containing the following elements.
- table opening and closing tag
	- tr tag for table rows
		- th for table header
		- td for table data

- useful feature for table: style attribute "border-collapse: collapse" 

## Units
- pixel -> good for border and small decorations, i.e. elements that should alwazs remains a specific size
- %
- vh, vw -> height and width of window 100 being maximum; similar to percentage but not tight to property and thus more versatile
- em -> based on relative size of font; changing font size affects em and em-based elements 
- rem -> good for keeping relative size and position of things when font size is changed

 -> use em sparingly, rem in most cases better
 -> use vh and vw over % as it can be used more explicitly

## Colors
- some are preconfigured and can be used referencing a name e.g. red
- colors can also be generated using rgb, hsl or hex
	- rgb = red, green, blue
	- hsl = hew, saturation, lightness
	- hex = hexadecimal-based code references representing rgb values
- good color resource including color coding and color pairings: [hue.tools](https://www.hue.tools)