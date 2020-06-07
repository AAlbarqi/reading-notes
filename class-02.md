# HTML TEXT

## HTML has six "levels" of headings:
`<h1>` is used for main headings
`<h2>` is used for subheadings
If there are further sections under the subheadings then the
`<h3>` element is used, and so on...

## Paragraphs
To create a paragraph, surround the words that make up the
paragraph with an opening `<p>` tag and closing `</p>` tag.

- `<b>` : makes characters appear bold.
- `<i>` : makes characters appear italic
- `<sup>` : contain characters that should be superscript
- `<sub>` : contain characters that should be subscript
- `<br />` : Line Breaks
- `<hr />` : Horizontal Rules
- `<strong>` :  indicates that its content has strong importance. 
- `<em>` :  indicates emphasis that subtly changes the meaning of a sentence
- `<blockquote>` : onger quotes that take up an entire paragraph.
- `<q>` : shorter quotes that sit within a paragraph.
- `<abbr>` : an abbreviation or an acronym.
- `<cite>` : to indicate where the citation is from (reference).
- `<dfn>` : indicate the defining instance of a new term.
- `<address>` :  to contain contact details for the author of the page.
- `<ins>` : show content that has been inserted into a document.
- `<del>` : show text that has been deleted.
- `<s>` : something that is no longer accurate or relevant.


## White Space Collapsing

When the browser comes across two or more spaces next to each
other, it only displays one space.

# Introducing CSS

| Selector  |  Example |
| ------------- | ------------- |
| Universal Selector  | `* {}`  |
| Type Selector  | `h1, h2, h3 {}` |
| Class Selector | `.note {}` `p.note {}`  |
| ID Selector  | `#introduction {}`  |
| Child Selector | `li>a {}`  |
| Descendant Selector | `p a {}`  |
| Adjacent Sibling Selector | `h1+p {}`  |
| General Sibling Selector | `h1~p {} ` |

## How Css Rules Cascade
- LAST RULE
   - If the two selectors are identical,the latter of the two will take precedence.

- SPECIFICITY
    - h1 is more specific than *
    - p b is more specific than p
    - p#intro is more specific than p

- IMPORTANT
    - You can add `!important` after any property value to indicate that it should be considered more important than other rules.


**Note** : CSS rules usually appear in a separate document, although they may appear within an HTML page.

# Basic JavaScript Instructions

**A script** is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a **statement**. 
`//` single comment, `/* */` multi-line comment

A script will have to temporarily store the bits of information it
needs to do its job. It can store this data in **variables**. 

`var name;`
`name = ' Jason';`

## DATA TYPES
JavaScript distinguishes between numbers, strings, and true or false values known as Booleans. 

## RULES FOR NAMING VARIABLES

1. The name must begin with a letter, dollar sign ($),or an
underscore (_). It must not start with a number. 

2. You cannot use keywords or reserved words. 

3. All variables are case sensitive.

4. Use a name that describes the kind of information that the
variable stores. 

5. If your variable name is made up of more than one word, use a
capital letter for the first letter of every word after the first word. 

**An array** is a special type of variable. It doesn't just store one value; it stores a list of values. 

`colors= ['white','black','custom']; `
 
`colors[2] = 'beige ' ;` Update the third item in the array

## OPERATORS

- ASSIGNMENT OPERATORS: Assign a value to a variable
`color = 'beige';`
- ARITHMETIC OPERATORS: Perform basic math
`area = 3 * 2;`
- STRING OPERATORS: Combine two strings
`greeting= 'Hi 1 + 'Mol ly';`
- COMPARISON OPERATORS: Compare two values and return true or false
`buy = 3 > 5;`
- LOGICAL OPERATORS: Combine expressions and return true or false
`buy= (5 > 3) && (2 < 4);`

# Comparison Operators :

- `==` is equal to
- `!=` is not equal to
- `===` strict equal to
- `!==` strict not equal to
- `<` less than
- `>` greater than
- `<=` less than or equal to
- `>=` greater than or equal to

# Logical Operators :

- `&&` logical AND
- `||` logical OR
- `!` logical NOT

- *Logical expressions are evaluated left to right.

## If statements

The if statement evaluates or checks a condition.

`if(hour< 12){`
   ` console.log('Good morning!');`
`}`
