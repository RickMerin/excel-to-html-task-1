# Excel to HTML Conversion

## Overview

This project involves converting an Excel spreadsheet to HTML with Bootstrap styling. The HTML table includes alternating row colors, merged headers, and proper numeric symbols.

## Deliverables

1. **Valid and Fast HTML**: The HTML file (`index.html`).
2. **Solution Outline**: An outline of the steps and tools used to convert the Excel file to HTML.

## Solution Outline

### 1. Convert Excel to HTML

1. Open the Excel file and save it in `.xlsx` format.
2. Export the file to HTML:
   - Convert the excel file to this site https://tableconvert.com/excel-to-html.
3. Clean up the HTML:
   - Remove any unnecessary tags to make the HTML clean and efficient also used semantic tags.

### 2. Add Bootstrap for Styling

1. Link to Bootstrap CSS in the `<head>` section of the HTML file:
   ```html
   <link
     rel="stylesheet"
     href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" />
   ```

### 3. External CSS for styling

1. Use CSS to apply styles:

   ```css
   body {
     font-family: Arial, sans-serif;
     font-size: 14px;
   }

   th {
     text-align: center;
   }

   td {
     text-align: right;
   }

   th:not(.dark),
   td:not(.dark) {
     color: green;
   }

   thead tr:nth-child(1) th {
     font-size: 18px;
   }
   ```

### 4. Style Headers and Numeric Symbols

1. Use Bootstrap classes or custom CSS to style headers:
   - Ensure headers are bold and visually distinct.
2. Ensure proper formatting for numeric symbols:
   - Use HTML entities or Unicode characters for special symbols as needed.

## Tools Used

1. **Microsoft Excel**: For opening and exporting the Excel file.
2. **Online Converter**: https://tableconvert.com/excel-to-html
3. **Text Editor/IDE**: VSCode.
4. **Bootstrap**: For styling the HTML.
5. **Web Browser**: Chrome, Firefox.

## File Structure

repo/
│
├── index.html
├── Readme.md
└── style.css
