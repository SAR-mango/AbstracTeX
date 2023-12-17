# AbstracTeX User Guide
## 1. Introduction
### 1.1 – Compile and Run the Program
To compile: `make`.

To run: `./abstractex`
### 1.1 Syntax
AbstracTex is a scripting language with four primary commands:
- `create` creates an object.
- `setup` sets up an object.
- `set` sets a parameter.
- `get` gets a parameter.
### 1.2 – Creating a Document
Upon running the program, you will be greeted with a shell interface.

To create a document:
``>> create document``

2. Page Formatting

2.1 – Margins and Page Numbers

2.2 – Headers and Footers

2.3 – Title, Section, and Subsection Formatting

3. Drawings

3.1 – Circuits

3.2 – Block Diagrams

3.3 – Simple Shapes

4. Graphs

4.1 – Functions

4.2 – Slope Fields

5. Tables

5.1 – Standard Data Tables

5.2 – Truth Tables

5.3 – Karnaugh Maps

6. Lists, Figures, and Columns

6.1 – Minipage Columns

6.2 – Figures and Captions

6.3 – Numbered and Bulleted Lists

equations
table of contents

## Example
```
create document
setup page style:
	set pages = all, not title
	set margins = 0.5in
	set lineSpacing = 1.25pt
	set indentFirst = false
	header:
		line 1:
			set left = "AbstracTeX"
			set right = "User Guide"
		line 2:
			set right = "Section " + get(currSection) + "." + get(currSubsection) + ": " + get(currSubsectionName)
	footer:
		center = "Page " + get(currPage) + " of " + get(totalPages)
setup title style:
setup section style:
setup subsection style:
```
- Page formatting, headers, and footers
- Title, section, and subsection formatting
- Table of contents
- Equations
- Drawings (circuits, block diagrams, simple shapes)
- Graphs (2D graphs of functions and direction fields)
- Tables (all sorts of them – truth tables, data tables, Karnaugh Maps...)
- Minipage columns
- Figures and captions
- Numbered and bulleted lists
