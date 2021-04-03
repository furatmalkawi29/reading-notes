# SMACSS and Responsive Web Design



## What's RWD?

### Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

<br><br>


## Flexible Layouts ?

 ### Flexible layouts, is the practice of building the layout of a website that's capable of dynamically resizing to any width, using relative length units, most commonly percentages or em units.

<br><br>


## Flexible Grid ?

## Demo:

### No matter how wide the parent container becomes, the layout scales proportionally.

<br><br>

```
section,
aside {
  margin: 1.858736059%; /*  10px ÷ 538px = .018587361 */
}
section {
  float: left;
  width: 63.197026%;    /* 340px ÷ 538px = .63197026 */   
}
aside {
  float: right;
  width: 29.3680297%;  /* 158px ÷ 538px = .293680297 */
}
```

<br><br>


## Media Queries

### Media query is a CSS technique introduced in CSS3.

### It uses the @media rule to include a block of CSS properties only if a certain condition is true.

<br><br>

![Drag Racing](https://www.seobility.net/en/wiki/images/6/6f/Media-Queries.png))

## Breakpoints ?

### With Media queries, We can add a breakpoint where certain parts of the design will behave differently on each side of the breakpoint.

### Example: switching from mobile screen to desktop at 768px 

<br><br>

## Floats

### Float is a CSS positioning property. 


![Drag Racing](https://i1.wp.com/css-tricks.com/wp-content/uploads/2021/03/print-layout.png?w=540&ssl=1
)

### Floats used to :
1.  ### wrap text around images
2.  ### create entire web layouts.


![Drag Racing](https://i2.wp.com/css-tricks.com/wp-content/uploads/2021/03/web-layout.png?w=540&ssl=1)

<br><br>

## Clearing the Float

### Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. Again an illustration probably does more good than words do.

<br>

```
#footer {
  clear: both;			
}
```

### Clear has four valid values as well.

### 1. Both: is most commonly used, which clears floats coming from either direction.

### 2. Left and Right can be used to only clear the float from one direction respectively. 
 
### 3. None is the default .
