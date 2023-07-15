# Data Cleaning
**Customer_order table:**
To start, we will remove all the ' ' values, and NULL from out Exclusions column as it might present a problem in the future when we try to do any analysis using it. We will do the same for the Extras by removing 'NaN'
and NULL values from the rows for the same reason. We want to make sure all data is consistent. 

![cust_orders](https://github.com/Sebsram/Case-Study---Pizza-Runner/assets/130475600/ca23e48e-1e36-4c95-88a8-57334f01c18e)

**Runner_orders table:**
For this table, just as before, we will cleaned all the null and ' ' (empty characters) in our columns. With the help of one PostgreSQL funtion: regexp_replace(column_name, '[a-z]+', '') We will change some of the values
to a string to make out analysis easier. To explain the function:
 1. regexp_replace: User for performing regular expression pattern matching and replace it with a string.
 2. Column_name: Represents the column we are trying to modify.
 3. [a-z]: Used for converting the characters to strings.
 4. 
![runner_orders](https://github.com/Sebsram/Case-Study---Pizza-Runner/assets/130475600/8bc44cab-b32f-481c-9a55-8121aa9aa359)

