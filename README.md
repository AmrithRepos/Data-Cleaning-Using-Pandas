This script processes a customer call list stored in an Excel file. It performs various data cleaning and transformation tasks to prepare the data for further analysis or use. The operations include removing duplicates, cleaning and formatting phone numbers, splitting address columns, and updating customer status indicators.

Script Description
Load Data:

Reads the customer call list from an Excel file located at C:\Users\amrit\OneDrive\Documents\Web Scrapping\Customer Call List.xlsx.
Data Cleaning:

Removes duplicate rows.
Drops an unnecessary column named Not_Useful_Column.
Strips unwanted characters from the Last_Name column.
Cleans and formats phone numbers by removing non-alphanumeric characters and adding hyphens for better readability.
Phone Number Formatting:

Converts the Phone_Number column to a string.
Formats the phone numbers into the XXX-XXX-XXXX format.
Removes any erroneous entries like "nan--" or "Na--".
Address Parsing:

Splits the Address column into Area, State, and Zip_code columns.
Drops the original Address column.
Customer Status Encoding:

Updates the Paying Customer and Do_Not_Contact columns to use 'Y' and 'N' for Yes and No, respectively.
Data Cleaning and Final Adjustments:

Replaces NaN values with empty strings.
Drops rows where Do_Not_Contact is 'Y' or Phone_Number is empty.
Resets the DataFrame index.
