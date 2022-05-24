# Programming & Java
- general division between programming languages: 
	- Machine: binary; only readable by humans with effort
	- Compliled: runs machine code and translates some
	- Interpreted: does not communicated directly with machine, hence easier to read 
- most dominant programming languages today
	- unix and c++
	- rust is taking over c++ as it was developed to be its successor
- most languages today are mix between compiled and interpreted
- imperative vs declarative programming language -> the first tells machine how, the latter tells machine only what to do

## JavaScript
- most popular programming language atm
- created by Mozilla in 90s
- not Java
- developed over time and influenced by Google's node js compiler 
- function: pre-written javascript that can be called upon by using shortcut
- can be used in html by using script tags
	- script tag can be placed anywhere in html but most common is head or as last child in body

## Java Functions
- alert(Text) -> shows popup
- document.write(Text) -> writes in document
- console.log(value1, value2) -> writes the specified values or bindings into the console log 
- functions always return values
- therefore a function call (console.log) can be used to call up a value

## Java Keywords
const - creates a constant or static binding, e.g. const noun1 = 'bear'
	- cannot be redeclared
- let - creates a non-constant or dynamic binding, e.g. let noun2 - 'apple'
	- can be redeclared, i.e. changed


## Primitive Values / Types
- Strings, e.g. "This is a string"
- numbers (in JavaScript always double-precision floating point numbers)
- Bolean, i/e. true or false
- null/empty: null or undefined (former is specifically set to that value, the latter is erroneously undeclared)

## Operators
- plus sign (+) -> overloaded operator, i.e. can be used not only as arithmentic operator to add up numbers but also to combine strings
- arithmetic operators: +, -, /, \*, \*\*, %
	- these are binary operators
- call operator ()
	- this is called variadic operator
- assignment operator =
	- also binary operator
- boolean operator: !
	- ! is unary operator
	- exclamation mark stands for 'not'
- equality operators: \==, !=
	-  these two are binary operator
	- double equal sign checks whether two values are equal and returns boolean value
	- exclamation mark plus equal sign means 'not equal'
- inequality operators: <, >, <=, >=

## Building MadLib
- necessary functions: 
	- prompt -> opens popup with text field for user to add text; like alert but alert has no input field
	- const Binding = prompt(Text)
- interpolation

## Revision
- **Bindings**
	- a pointer or reference to a value in memory
	- Declarations
			- const -> cannot be reassigned
			- let -> can be reassigned
			- var -> can be reassigned; different (and older than const and let)
			- in general, use let and const
	- Rules for creating binding: start with a letter, underscor or dollar sign; after first letter, can use number, letter, underscore, dollar sign; don't use any of JavaScript's reserved keywords (see below)
- **Values**
	- Primitive Values
		- Strings -> denote string literal with single or double quotation marks or back tick
		- Numbers -> denote a number literal by using decimal digits and/or point/period 
		- Boolean -> denote a Boolean literal by using keywords true or false
		- null/empty-types -> denote a null/empty type by using null for value left intentionally empty; do not use undefined anywhere yourself
	- Non-primitive Values (tbd)
	- Value vs Literal
		- both values and literals: 12345; "this is a string"; false; null
		- values but not literals: aBinding (defined as const aBinding="this is a string")
- **Funtions**
	- pre-defined block of statements that you can call, you can pass arguments into (if paramenters are in the function definition), and will always have a single return value (even if `undefined`)
	- call a function with the call operator, i.e. quotation marks, eg. alert(); pass in arguments (if expected), e.g. alert('This is a text')
	- Arguments: values that a function takes, of a type that was specified when the function was defined
- **Operators**
	- a function (essentially) that is built into the lanuage and has "language support". An operator also takes arguments and always return a single value
		- e.g. call operator, assignment operator, ...
	- **overloaded operator**: is one that changes its behavior depending on the types of values passed to it, e.g. plus sign can be used to combine strings or to add up numbers 

- string interpolation: using back ticks with string allows the use of ${binding} which can be used to call a value 

- **Functions**
	- window.alert (or simply alert)
	- window.prompt (or simply prompt)
	- document.write
	- console.log
-  **Keywords**
- 
	- let
	- const
	- var
	- true 
	- false
	-  null
	- 