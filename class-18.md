# Responsive Web Design and Regular Expressions
# CSS Grid

CSS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system.

###### Properties for the Parent (Grid Container)
**display**
Defines the element as a grid container and establishes a new grid formatting context for its contents.

Values:
- grid – generates a block-level grid
- inline-grid – generates an inline-level grid

- grid-template-columns
- grid-template-rows
Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.

Values:
- <track-size> – can be a length, a percentage, or a fraction of the free space in the grid (using the fr unit)
- <line-name> – an arbitrary name of your choosing

![](https://css-tricks.com/wp-content/uploads/2018/11/template-columns-rows-01.svg)

- grid-template-areas

Values:

- <grid-area-name> – the name of a grid area specified with grid-area
- . – a period signifies an empty grid cell
- none – no grid areas are defined

![](https://css-tricks.com/wp-content/uploads/2018/11/dddgrid-template-areas.svg)

- grid-template
A shorthand for setting grid-template-rows, grid-template-columns, and grid-template-areas in a single declaration.

![](https://css-tricks.com/wp-content/uploads/2018/11/dddgrid-gap.svg)

###### Properties for the Children (Grid Items)
- grid-column-start
- grid-column-end
- grid-row-start
- grid-row-end

**Note:**
float, display: inline-block, display: table-cell, vertical-align and column-* properties have no effect on a grid item.

- grid-area
Gives an item a name so that it can be referenced by a template created with the grid-template-areas property. Alternatively, this property can be used as an even shorter shorthand for grid-row-start + grid-column-start + grid-row-end + grid-column-end.

Values:
<name> – a name of your choosing
<row-start> / <column-start> / <row-end> / <column-end> – can be numbers or named lines.

![](https://css-tricks.com/wp-content/uploads/2018/11/grid-area.svg)
