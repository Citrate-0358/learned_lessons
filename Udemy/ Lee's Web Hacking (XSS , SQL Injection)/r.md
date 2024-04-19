
# Using XAMPP with MySQL Database and phpMyAdmin

## Database Connection
- To access MySQL database using XAMPP:
    ```bash
    mysql -u root -h localhost -p
    ```

- Enter your password when prompted.

## Basic MySQL Commands
- Show available databases:
    ```sql
    show databases;
    ```

- Use a specific database:
    ```sql
    use databasedb_name;
    ```

- Show tables in the current database:
    ```sql
    show tables;
    ```

- Describe a table structure:
    ```sql
    desc itembox;
    ```

- Select specific columns from a table:
    ```sql
    select name, product from itembox;
    ```

## XSS (Cross-Site Scripting)
```html
<script>alert("hey guys");</script>

# Using XAMPP with MySQL Database and phpMyAdmin

## Database Connection
- To access MySQL database using XAMPP:
    ```bash
    mysql -u root -h localhost -p
    ```

- Enter your password when prompted.

## Basic MySQL Commands
- Show available databases:
    ```sql
    show databases;
    ```

- Use a specific database:
    ```sql
    use databasedb_name;
    ```

- Show tables in the current database:
    ```sql
    show tables;
    ```

- Describe a table structure:
    ```sql
    desc itembox;
    ```

- Select specific columns from a table:
    ```sql
    select name, product from itembox;
    ```

## XSS (Cross-Site Scripting)
```html
<script>alert("hey guys");</script>

##Defensive Measures
Use strip_tags() as a filter to remove HTML tags:
Reference: PHP Manual - strip_tags()
Implement SQL Injection Prevention:
Sanitize user inputs.
Avoid directly inserting user inputs into SQL queries.
Example queries:
```php
$query ="insert into itembox(date ,name ,product ,price ,screenshot,approved)values(NOW(),'$name','$product','$price','$screenshot',false)";

###Examples of SQL Injection
Using common SQL injection strings:
Username: 1' or '1'='1
Password: 1' or '1'='1
Bypassing authentication:
Username: admin'--
Password: anything
###Additional Resources
Demo Test Website - demo.testfire.net
Vulnerable PHP Test Site - testphp.vulnweb.com
###Additional PHP Functions
trim(): Used to remove whitespace or other predefined characters from the beginning and end of a string.
is_numeric(): Checks whether a variable is a number or a numeric string.

