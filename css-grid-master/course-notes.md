#CSS Grid Course Notes

##Terms

Tracks - a collection of columns and rows

display: grid; - declares a grid for an element

grid-template-columns - declares number and size of columns


grid-template-rows - declares number and size of rows

grid-gap - creates space between columns and rows. Like margin

repeat() - takes two arguments. How many times to repeat, and the size. Example repeat(5, 100px)

grid-auto-rows - controls implicit rows


##Concepts

Whenever you declare a CSS Grid "container" you make all of its direct children into "items" in the grid

Values can be pixels, rem, fr (which replaces percentages), and auto

CSS Grid is hard to visualize because the borders and stuff are not stated. Use Firefox dev tools to see it visually

In Firefox turn line numbers on to see numbers

Tracks are numbered by the lines that start and stop them. So there will always be one more number than the number of a column or row

In dev tools dotted lines are for implicit grid, dark dashes are for explicit grid

Firefox won't allow multiple values for implicit rows. Chrome will

By default an overflow of items will produce more implicit rows