# ZC Spreadsheet Sort
A function, written in R, designed to scan spreadsheets and sort the values in one specified column by the values in another specified column

# Purpose
This function returns a dataframe where the column names are the unique values in the spreadsheet's "categories_column" (specified in the function), and the values in each column are the unique values in the spreadsheet's "subcategories_column" (specified in the function) that coorespond to values in the spreadsheet's "categories_column". 

There are two functions: scan.group() and scan.numbers(). The only meaningful difference between them is that scan.group() returns unique values in the subcategories column while scan.numbers() returns all targeted values regardless of reepition. 

# Arguments
 1. "spreadsheet" = a dataframe containing data to be sorted. 
 2. "categorization_vector" = an array of categories by which to sort the data
  - The categorization_vector will be the dataframe's column names 
 3. "categories_column_position" = a numeric value denoting the position of the column containing the values
   by which spreadsheet will be sorted
  4. "subcategories_column_position" = a numeric value denoting the position of the column containing the values
   that will be sorted 
   - The values in this column will make up the values in the dataframe 
