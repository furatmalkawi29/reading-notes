
# Objects

## What's object?

- Object is  a set of variables and functions

- it **models things  from the real world** : students , employees , shop branches 


![](https://www.pngkit.com/png/detail/118-1189654_college-students-college-student-illustration-png.png)

*** 
***

## Properties and methods?

<br>

- in objects :
  -  Variables  named as : **Properties**
  - Function named as : **Methods**


- **Properties** tell us information about the object .
- **Methods** perform tasks associated with the object . 

<br>

- Properties and methods are example :  **(key: value) pairs** 

<br>

- **Key** : name of property/ method 
- **Value** : <br>
In property --> string, boolean , number, array , another object ( Nested Object)
<br>
method --> function 

***

## Litral Notation 
- one of the ways to create an object (Constructor notation is another way)

![201/r7.PNG](https://github.com/furatmalkawi29/reading-notes/blob/main/201/r7.png?raw=true) 

## Accessing Object 

### 1. Dot Notation
- Accessing properties /methods 
- **Example:** 

```
hotel.name;

hotel.checkAvailability ( );
```

### 2. Braket Syntax 
- Accessing properties only  
- used when property name is a number 

- **Example:** 

```
hotel.['name'];

```

***

# Document Object Model 

### - As browser loads web page, it creates a model of that page. 

### - The model is called a DOM tree, Its stored in browsers' memory.

*** 
<br>

### Every element, attribute, and piece of text in the HTML is represented by its own DOM node. 

### Each node is an object with methods and properties. 

### 1. document node 

- **Top** of the DOM tree .
- Represents the entire page . 
- Used to access any element, attribute, or text node : **Its the starting point for all visits to the DOM tree**

<br>

### 1. Element node
- All HTML elements 
- Methods allows accessing element nodes 
- After accessing it, we can altr its text and attribute nodes .

<br>

### 2. Attribute node
- Attribute nodes **are not children** of the element they are part of it .

### 3. Text node  
- The Text within an element is
stored in seprate text node. 
- Text nodes **cannot have children.**

![](https://github.com/furatmalkawi29/reading-notes/blob/main/201/r6.png?raw=true)

##  DOM queries

### - methods that **finds elemnts in DOM tree** (access elemnts)

### Example: 

```
 getElementById ();

 getElemnetByClassName ();
```

### - Whenever a DOM query can return more than one node, it will always **return a Nadel list**. 

***

### Catching DOM Query 

- `getElementById ();` **gets reference of element** , not the element itself .

- Saving that reference in a variable called **catching query** 

<br>
<br>

*** 

## Methods that select Individual Elements (return one element)

They have same syntax .
### 1. getElementById ( )

### 2. querySelector ( )

<br>
<br>

## Adding/ Removing HTML content 

### 1. innerHtml property (fast,unsafe)

- Adds **both Text and Tags (Markups) in one line** to the selected element .

- Adds **content as string**, get it as a string also . 
<br>

- Syntax: 

```
document.getElementById('one').innerHtml = 'Hello <b>World</b>' ;
```

### 2. DOM Manipulaton (slow, safe)
### Uses multiple steps and a method for each step .

![](https://github.com/furatmalkawi29/reading-notes/blob/main/201/r5.png?raw=true) 


1. Create New Element Node .

```
newElement = document.createElement('h1');
```

2. Find the Element Node that you want to add the new element to as a child .

```
parentElement = document.getElementByID('div1');
```

3. Append child element to the found parent element .

```
parentElement.appendChild(newElement);
```

4. Add Text node using method or property 

```
newElement.textContent = 'hello world' ;
```

<br> 
<br> 

*** 
## Remove Html content 
1. Find the Element Node that you want to delete

```
deletedElement = document.getElementByID('tr5');
```

2. Find the Parent of the Element Node that you want to delete 

```
parentElement = document.getElementByID('table1');
```

3. Use removing method .

```
parentElement.removeChild(deletedElement);
```

<br>

*** 

## Attribute Node 

### Working on Elements Attribute done using multiple methods :

### 1. hasAttribute( )
  
  Checks if the element has a certain attribute or not .

### 2. getAttribute ( )

Returns the value of a certain attribute 

### 3. setAttribute ( )

Creats an attribute for the element (if it didnt exist) and sets a value to it .

### 4. removeAttribute ( )

Removes attribute 