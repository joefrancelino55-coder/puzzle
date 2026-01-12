# Code Documentation

# Tutorial: Number Puzzle (HTML/JS)

This project implements a small logic game presented within a table. The user can start by filling the table with unknowns (indicated by "?") and play by interacting with the table cells to make substitutions.

## Overview
- Generates a grid (table) with 10 rows and 13 columns.

- The cells contain numbers, operators, and symbols, with some positions marked by `?` to represent unknowns.

- When clicking on a cell:

- First click selects the cell (highlighted).

- Second click copies the content of the second cell to the first.

- A "Reload" button reloads the page, generating a new grid.

## Content Structure (High Level)

- HTML:

- Basic structure with `<table id="my-table">` for the grid.

- A button that reloads the page.

- CSS:

- Grid appearance: size, colors, borders, hover, etc.

- JavaScript:

- Signal/operator constants.

- Generation of the `matrix` (10x13) array with content patterns.

- Insertion of 5 `?` in random positions per row.

- Construction of the table in the DOM from the array.

- Click logic on cells to select/copy content between cells.

## How the code "plays" (game rules)

- The grid contains numbers, operators, and symbols, forming incomplete expressions.

- The unknowns `?` can be replaced with values ​​during the game, allowing the player to complete the expressions.
