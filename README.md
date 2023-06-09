# Table Cleanup
HTML Table editor that provides scoping and a visual editor so that the table meets [Canada.ca web standards](https://www.canada.ca/en/government/about/design-system.html) and the latest [Web Experience Toolkit (WET)](https://wet-boew.github.io/wet-boew/index-en.html) Style guidelines.

**This tool is actively used to code tables in the [Federal Budget](https://www.canada.ca/en/department-finance/services/publications/federal-budget.html) and other Finance Canada publications.**

The table output complies with TBS guidance found here: https://wet-boew.github.io/wet-boew-styleguide/design/tables-en.html

This project is regularly updated twice a year when performing critical analysis review for the Department of Finance's major reports: Federal Budget, and Economic and Fiscal Update (EFU) or Fall Economic Statement (FES).

## Upcoming
* Complex (ID and headers) scoping helper

## Features
* Interactive editor
* Horizontal alignment
* Indent
* Merge cells
* Bolding
* Toggle header row
* Create table footer
* Drag selection
* Simple Scoping

## Instructions
1. Open `index.html`
2. Once you copy the `<table>` code from your HTML source, paste it and overwrite the contents in the HTML Input box
3. Press the Clean up button
4. Click on cells within the table of the **Designer** to show the toolbar

## Requests and Issues
Please feel free to create in Issue [on Github](https://github.com/jordan-chou/table-cleanup/issues) to make a request or flag issues.

## Options
**Scope Table**: Adds scope attributes for row and column headings. On by default.

**Financial table**: Aligns all cells to the right except for row headings. Great for tables with numerical data. On by default.

**Remove bold in rows**: Attempts to remove bold for row headings. May not work depending on how the bolding is implemented. On by default.

**Trim spaces**: Removes non-breaking spaces and double spaces in row headings. On by default.

**Move last row to footer**: Moves the last row of the table to the table footer. One will be created if none exists. Useful for tables where `tfoot` content is the last row of the `table`.

**Add empty footer**: Adds an empty footer to the table. Useful for tables where the `tfoot` content is outside the `table` tags.

**French number format**: _Experimental option_. Style numbers into French format, mainly for thousands and decimal separators. Replaces all whitespace thousands separators with non-breaking space and all dot decimal separators with a comma.

## Known issues
### Drag selection (Added March 2023)
* Drag selection in the Designer may not work when selecting a merged cell (cell with colspan > 1)
* Releasing the mouse outside the Designer will not complete the drag selection. You **must** release within the table
* Cannot deselect cells. You must click on a single cell to deselect it or press the Deselect all button in the toolbar

## About

### What was this project's initial purpose?
This tool was initally created for the Department of Finance to automate the scoping process for increased accessibility. Additionally, complex HTML tables were very time-consuming to code, so the tool was later expanded so that tables can be modified within the webpage. This project has **greatly** decreased coding time for any report or publishing task. Prominent tool used for publishing the Canadian Federal Budget.
  
### When was it created?
This project started in 2021 during my co-op term with Department of Finance. I am the sole developer on this project and I have been upgrading, expanding, and maintaining it since then.
  
### What was my experience at the time?
I had a little bit of JavaScript and HTML experience at the time. In retrospect, I think I did a good job with the tool in terms of code design but it definitely can and should be refactored. However, in its current state, functional programming help divide the individual features.

### Contact
Please feel free to reach out to me for feedback, issues, or requests at jordan.chou@fin.gc.ca.
