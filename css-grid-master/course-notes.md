#CSS Grid Course Notes

##Terms

Tracks - a collection of columns and rows

display: grid; - declares a grid for an element

grid-template-columns - declares number and size of columns


grid-template-rows - declares number and size of rows

grid-gap - creates space between columns and rows. Like margin

repeat() - takes two arguments. How many times to repeat, and the size. Example repeat(5, 100px). The first argument repeats the pattern in the second - repeat(2, 1fr 2fr) = 1fr 2fr 1fr 2fr

repeat() function can be used multiple times within template list - 50px repeat(50px 1fr 25px)

grid-auto-rows - controls implicit rows

grid-auto-flow - default is row. If changed to column it overflows items into inplicit row columns

using percentages won't account for margin. 50% 50% will add to 100% of the space place margin

"fr" unit - fractional or "free space". Splits up free space left after all the elements are laid out

default width of element is the viewport. Default height is the content within

unless I define a height of the grid, "fr" for row won't do anything. There's no free space

auto - match the space with the content

grid-coloumn-start / end - control where an items starts and ends

auto-fit - make as many coloums as can fit a track

##Concepts

Whenever you declare a CSS Grid "container" you make all of its direct children into "items" in the grid

Values can be pixels, rem, fr (which replaces percentages), and auto

CSS Grid is hard to visualize because the borders and stuff are not stated. Use Firefox dev tools to see it visually

In Firefox turn line numbers on to see numbers

Tracks are numbered by the lines that start and stop them. So there will always be one more number than the number of a column or row

In dev tools dotted lines are for implicit grid, dark dashes are for explicit grid

Firefox won't allow multiple values for implicit rows. Chrome will

By default an overflow of items will produce more implicit rows

Item take up entire explicit grid:
grid-column: 1 / -1
grid-row: 1 / -1

What's the difference between 1fr and auto? Both stretch to fit content

Giving an item a fixed width with widen the whole column. Use span make content cross over into more than one grid spot

If I use grid-column then it will default to grid-coloumn-start / end values. I can see this in Dev Tools

grid-column: 1 / -1; is like making width 100%

grid-column can take span alone, start and end positions, or positions plus span

## Resources

Card Layout - https://getflywheel.com/layout/card-layout-css-grid-layout-how-to/

Jen Simmons - https://labs.jensimmons.com/

CSS Grid Garden - http://cssgridgarden.com/