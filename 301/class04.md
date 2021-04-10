# CSS Grid 

## CSS Grid is a powerful tool that allows for two-dimensional layouts to be created on the web. 

<br>

# Properties for the Parent (Grid Container)

# - display
Defines the element as a grid container and establishes a new grid formatting context for its contents.

### - Values:

**grid** – generates a block-level grid

**inline-grid** – generates an inline-level grid



# - grid-template-columns and grid-template-rows

### - Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.

### - Values :

1. track-size – can be a length, a percentage, or a fraction of the free space in the grid (using the fr unit)

- The fr unit allows you to set the size of a track as a fraction of the free space of the grid container.

2. line-name – an arbitrary name of your choosing


## - grid-template
A shorthand for setting grid-template-rows, grid-template-columns, and grid-template-areas in a single declaration.


![](https://css-tricks.com/wp-content/uploads/2018/11/dddgrid-gap.svg)


# Properties for the Children (Grid Items)

## -grid-column-start
## -grid-column-end
## -grid-row-start
## -grid-row-end
Determines a grid item’s location within the grid by referring to specific grid lines. 


## -Values:

1. line  – can be a number to refer to a numbered grid line, or a name to refer to a named grid line

2. span number - the item will span across the provided number of grid tracks

3. span name – the item will span across until it hits the next line with the provided name

4. auto – indicates auto-placement, an automatic span, or a default span of one

## - Example :
```css
.item-a {
  grid-column-start: 2;
  grid-column-end: five;
  grid-row-start: row1-start;
  grid-row-end: 3;
}
```

![](https://css-tricks.com/wp-content/uploads/2018/11/grid-column-row-start-end-01.svg)


