# This is a QUERIES study !
## start
* * *
### **Selct**

    SELECT column1, column2 
    FROM table_name;
* * *
### **As**
**AS** is a keyword in SQL that allows you to rename a column or table using an alias.       

    SELECT name AS 'Titles'
    FROM movies;

* When using AS, the columns are not being renamed in the table. The aliases only appear in the result.
* * *

### **Distinct**
**DISTINCT** is used to return unique values in the output.      
 It filters out all duplicate values in the specified column(s).

    SELECT DISTINCT tools 
    FROM inventory;
***
### **WHERE**
We can restrict our query results using the **WHERE** clause in order to obtain only the information we want.    

    SELECT *
    FROM movies
    WHERE imdb_rating > 8;

1.**WHERE** clause filters the result set to only include rows where the following condition is true.   
2.imdb_rating > 8 is the condition. Here, only rows with a value greater than 8 in the imdb_rating column will be returned.    
***

### **LIKE**
**LIKE** can be a useful operator when you want to compare similar values.   

    SELECT * 
    FROM movies
    HERE name LIKE 'Se_en';

* **LIKE** is a special operator used with the **WHERE** clause to search for a specific pattern in a column.    
* **name LIKE 'Se_en'** is a condition evaluating the **name** column for a specific pattern.    
* **Se_en** represents a pattern with a wildcard character.     
***


    SELECT * 
    FROM movies
    WHERE name LIKE 'A%';     

**%** is a wildcard character that matches zero or more missing letters in the pattern. For example:   
* **A%** matches all movies with names that begin with letter ‘A’    
* **%a** matches all movies that end with ‘a’     
***

    SELECT * 
    FROM movies 
    WHERE name LIKE '%man%';       

any movie that contains the word ‘man’ in its name will be returned in the result.   
***
### **BETWEEN**
The **BETWEEN** operator is used in a **WHERE** clause to filter the result set within a certain *range*.    
It accepts two values that are either numbers, text or dates.       
    SELECT *
    FROM movies
    WHERE year BETWEEN 1990 AND 1999;    












