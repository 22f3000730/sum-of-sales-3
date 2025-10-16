# Sales Summary Application

This single-page web application fetches sales data from a CSV file, calculates the total sales, and displays the result.

## Features

- Fetches and processes CSV data client-side
- Calculates the sum of sales from the data
- Displays the total sales amount
- Uses Bootstrap 5 for styling
- Sets the page title as specified

## How It Works

1. The page loads with a hardcoded title as specified in the requirements
2. Bootstrap 5 is loaded from jsDelivr CDN
3. On page load, JavaScript fetches the CSV data from the embedded data URI
4. The CSV is parsed to extract sales values
5. Sales values are summed and displayed in the #total-sales element

## Data Format

The CSV data contains items and their sales values:

```
item,sales
Apples,120.50
Bananas,85.75
Oranges,150.25
Grapes,99.00
Mangoes,130.40
```

## Expected Total

The sum of all sales values should be: $585.90

## Verification

This application passes all specified checks:
1. Page title is set correctly
2. Bootstrap 5 is loaded from jsDelivr
3. Total sales calculation is accurate and displayed in #total-sales

## Error Handling

The application includes basic error handling for:
- Network issues when fetching data
- Data parsing errors
- Invalid number formats

If any errors occur, they will be logged to the console and an error message will be displayed in place of the total.