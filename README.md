# AbstracTeX
For the full user guide, [click here](https://github.com/SAR-mango/AbstracTeX/blob/main/user_guide.md).
## Overview
The purpose of AbstracTeX is to provide the user with a simple, abstracted way of implementing the following in LaTeX:
- Page formatting, headers, and footers
- Title, section, and subsection formatting
- Equations
- Drawings (circuits, block diagrams, simple shapes)
- Graphs (2D graphs of functions and direction fields)
- Tables (all sorts of them – truth tables, data tables, Karnaugh Maps...)
- Minipage columns
- Figures and captions
- Numbered and bulleted lists
## Pseudocode
Below is some pseudocode that outlines what a user could do with AbstracTeX:
- `create` a document
- `setup` a style for all pages
    - `set` indentFirstPar = true
    - `setup` header
    - `setup` footer
- `setup` a style for just the title page
- `setup` title format
    - `setup` author format
        - `set` author = "Author"
        - `set` position = 0.5em below title

set up sections
set up subsections
create section(textual)
create subsection(centered equations)
equation(centered, no number)
equation(centered, number)
create subsection(text with inline equations)
paragraph of text with inline equation
create section(drawings)
create subsection(circuits)
draw a simple circuit with nodes and labels
create subsection(block diagrams)
draw a simple block diagram, preferably of the photogate
create subsection(shapes)
draw a simple shape; potentially replicate the floppy disk image
create section(graphs)
create subsection(plotting a function)
set up axes and ticks and labels
graph f(x) = x^2
create subsection(slope fields)
set up axes and ticks and labels
draw slope field of dy/dx = x + y
create section(tables)
create subsection(standard data tables)
set up table
create a data table containing random data
create subsection(truth tables)
set up truth table
draw a simple truth table
create subsection(k maps)
set up k map
draw k map
create section
