
 <div  style="font-size:160px; background-color:pink; text-align:center;"> <h1> <br><b> TEXT </b> <br><br> </h1> </div>

# When creating a web page, you add TAGS 

## Tags known as: **MARKUPS**

## This chapter will cover **Text Markups**
<br><br>
***
<br>

## 1. **Structural markup:**

### Allow browsers to show users the appropriate structure for the page. It describes the structure of page .

<br>

## 2. **Semantic markup:**

### Doesn't affect the structure of web pages . Provides extra information and meaning and description of content .


# -------------------------------------

# Structural markups :

![](b1.PNG)

<br>

## 1.Headings

* HTML has six "levels" of
headings 

* `<h1> <h2> .....<h6>`
* `<h1>` : main headings
* `<h2>` : subheadings

<br>



## 2.Paragraphs
  `<p> your paragraph ..... </p>`
* browser will show
each paragraph on a new line
with some space between it and
any following paragraphs.

<br>

![](b3.PNG)

## 3. Bold 

 * `text <b> bold texts... </b> text`
 * Make characters appear bold.
 * Used for Keywords 
* Does not imply
any additional meaning.

<br><br>

## 3. Italic

 * `text <b> bold texts... </b> text`
 * Make characters appear bold.
 * Used for 
   - Technical terms
   - Names of ships,
   - Foreign words

<br>

![](b4.PNG)


## 4. Super-script and Sub-script
  
  * ## Superscript 
  * ` The 4<sup>th</sup> of October`
  * Contain characters slightly **above** the normal line 
   * suffixes of dates or mathematical concepts like (power)

  * ## Subscript 

   * ` The H<sub>2</sub>O`
  * Contain characters slightly **below** the normal line 
   * Chemical formulas such as H20 

   <br>

![](b5.PNG)

<br>

# White Space 

## What's White Space?

* a Text composed only of spaces, tabs or line breaks 

![](b6.PNG)

<br>

## What's White space collapsing?
* browser completely **ignore** white spaces .

* **Two or more spaces** next to each
other ----> only **one space displayed** 

* **linevbreak** ----> only **one space displayed** 

* ## **Makes code easier to read** 

![](b7.PNG)

# result:

![](b8.PNG)

<br>

## 5.Line Breaks and Horizontal Rules

* `<br>` Add a line break inside the
middle of a paragraph 
* `<hr>` add a ruler . Used as a break .

 <br>
 <br />

# Empty elements 
* elements that
do not have words between
an opening and closing tag.
* Like `<img> , <br> , <hr>`
* **GOOD PRACTICE** : add space and a forward slash 
like : 
* `<br> same as <br />` 

<br><br><br>


# 2. **Semantic markup:**

* ## Purpose : **Describe the content** of your web pages 

<br>

* ## **Shouldn't** use them to **change** the way that your text looks .

<br>


* ## **WHY?** : Used for programs like screen readers or search engines .

<br>


 * ## **HOW?** They use the extra information. For example: 
- ### voice of a screen reader may add emphasis to the words inside the <em> 
- ### search engine might register that the page has a quote if you use the <blockquote> 

<br>

![](b9.PNG)

<br><br>

## 1.Strong & Emphasis
* `<strong> </strong>`
* indicates that 
content has strong importance

* will show
the contents in bold 

<br>

* `<em> </em>`
* Changes
the meaning of a sentence (depending on what word 
in the sentence is Italic).

* will show
the contents in italic 

<br>

![](b10.PNG)

<br><br>


## 1.Qoutations 

### used for marking up quotations:
* `<blockquote> </blockquote>`
* used for longer quotes that **take
up an entire paragraph**.

* `<p>` tag still used inside .
* it  indent the paragraph (push it away . adds a margin)

<hr>
<br>

![](b11.PNG)


* `<q>  </q>`

*  used for
shorter quotes 

*  most browsers put quotes around
the content 

<br>

![](b12.PNG)

<br>

## 2.Abbreviations & Acronyms  
* `<abrr> </abbr>`
* Used for Abbriviations (eg. Doctor - Dr ) and Acronyms (eg. USA - United States of America) 

* It shows a description when you mouse over the element.
* Needs "title=" attribute .

![](b13.PNG)



## 3.Citations & Definitions 
* `<cite> </cite>`
* Used when mentioning a book name, movie, name of a published paper 
* content will appear italic 
* `<cite>A Brief History of Time</cite> by Stephen
 Hawking has sold over... `

<br>

  * `<dfn> </dfn>`
  * Used when defining new term 
  * `A <dfn>black hole</dfn> is a region of space`

<br> 

## 4.Author Details  
 * contain
contact details for the author of
the page (his address, email, phone number).

* `<address>  742 Evergreen Terrace, Springfield.</address>`

<br> 

## 5.Changes to Content

  * `<ins>  </ins>` 
  * used
to show content that has been
inserted into a document
* appears Underlined

<br>

* `<del>  </del>`

* to show deleted text 
* appears with a line crosssing though it 

<br>

* `<s>  </s>`
*  indicates
something that is no longer
accurate or relevant
* appears with crossed line

![](https://static.javatpoint.com/htmlpages/images/html-del-tag2.png)

<br><br>


<div  style="font-size:160px; background-color:pink; text-align:center;"> <h1> <br><b> CSS</b> <br><br> </h1> </div> 

# What Does CSS Do?

## CSS allows you to create **rules** that specify how the **content of an element should appear** .

<br><hr>


# How CSS works?

## The key to understanding how CSS works is to imagine that there is an **invisible box around every HTML element** .

<br>

## BLOCK & INLINE ELEMENTS
Every HTML element has a default display value, depending on what type of element it is.
<br><br>

There are two display values: block and 
<br><br>

* **Block level elements** : 
* always start on a new line . 
* Takes up the full width available . 
* Has default TOP and BOTTOM Margin (16px) .
*  `<h1>-<h6>, <p> and <div>` 

![](b14.png)

<br>

* **Inline elements**: 
* Does not start on a new line (flow within the
text)
* only takes up as much width as necessary.
* doesn't have a default margin .
 
* `<b>, <i>, <img>, <em> and <span>`

![](b15.png)

<br>


# Style Rules
## * These rules govern how element's content should be displayed. 

<br>

## * A CSS rule contains two parts: 
## 1.**selector**: indicate which element the rule applies to .

## 2.**declaration**: how the selected elements should be styled.

<br>

##  **Declarations**  sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon

<br>

![](b16.PNG)

<br>



<div  style="font-size:160px; background-color:pink; text-align:center;"> <h1> <br><b> JavaScript</b> <br><br> </h1> </div> 


# What is a script?

* A script is a series of instructions that a computer can follow step-by-step to achieve a goal. 

* You could compare scripts to : RECIPES , HANDBOOKS, MANUALS .


![recipe](rec.jpg)


# How do I creat a Script?

<br>

## 1: DEFINE THE GOAL

To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it. 

## 2: DESIGN THE SCRIPT

You can use flowcharts to work out how the tasks fit together. The flowcharts show the paths between each step.

<br>

![](img1.PNG)

3: CODE EACH STEP

<br> <br>

# EXPRESSIONS

  An expression results in a single value. There are two types of expressions:
  <br>

### 1.EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE: 

<br>

`var color = 'beige' ;`


### 2.EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE:

<br>

`var area = 3 * 2;`

# OPERATORS 
Expressions rely on operators to calculate a value.

<br>

### 1.ASSIGNMENT OPERATORS

`color = 'beige';`

### 2.ARITHMETIC OPERATORS

`area = 3 * 2;`

### 3.STRING OPERATORS

`greeting= 'Hi 1' + 'Mol ly'`

### 4.COMPARISON OPERATORS

`buy = 3 > 5;`

### 5.LOGICAL OPERATORS

`buy= (5 > 3) && (4>2);`

<br><br>


# Comparsion Operators 

## Here are the common comparsion operators in programming:

<br> <br>

## 1.Less than (<) 

## 2.Greater than (>) 

## 3.Less than or equal to (<=) 

## 4.Greater than or equal to (>=) 

## 5.Equal to (==) 

## 6.Not equal to (!==)

## 7.Strict Equal to (===)

## 8.Strict Not Equal to (!==)


<br><br>

# Logical Operators 

## Here are the common Logical operators in programming, they usually return True or False

![](img11.PNG)

# 1.|| (Logical OR)

In classical programming, the logical OR is meant to manipulate boolean values only. If any of its arguments are true, it returns true, otherwise it returns false.

# 2.&& ( Logical AND)

In classical programming, AND returns true if both operands are truthy and false otherwise

# 3.! (Logical Not)

* Converts the operand to boolean type: true/false.
* Returns the inverse value.

<br>
<br>

# Loops

## 1.For Loop

### Used if you need to run a code  a specific number of times .

## 2.While Loop

### Used if you don't know how many times the code should run.

## 3..Do While 

### Similar to While . It will always run the statement at least once even if the condition is false.

<br>

# Loop Counters 

For uses counters as a condition, this allows it to run a specified number of times .

## Condition made of 3 statements:
1. Initialization
2. Condition
3. Update



## SWITCH STATEMENTS

A switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value. 
