# Raw-dataset-cleaning
1.	Auto fitting rows and columns
The data is not visible properly so we will auto fit the rows and columns by using these two shortcuts : Alt+H+O+I for column and Alt+H+O+A for rows.

2.	Find & Replace
The Client column has very long names so we will shorten them such that we will not have anything in the parenthesis. For this we will use the Find & Replace shortcut (Ctrl+H). In the find value we will insert : (*), in order to get rid of anything that is between those parenthesis and then select replace all.


3.	Converting into lowercase
The client names are all in capital letters which makes it hard to read so we will convert them into small letter using the function LOWER(). We will create a new column and name it as client. After converting the first cell value into lower case we’ll double click at the end of the converted cell which will convert and copy all the values from the previous client column into the new one.

4.	Referencing and pasting formula as values
Now we have two same columns named as Client so we will delete one of them. But it shows error as the previous column is referencing the new one. So now we will select and copy all the cells of the new column and paste them as value using the shortcut Alt+H+V+V and then we will delete the old column using Ctrl+minus.


5.	Removing irregular space and properly casing the words
The Contact column has irregular spaces and improper cases. So we will create a new column and will use the formula TRIM(PROPER(D3)) in order to remove the spaces and properly case the words. Now we have two same columns, so we will delete the old improper one.

6.	Text to Column
In the department column, along with department names region is also mentioned parting them using underscore. So we will create a new column named region. Then follow these steps:
1. Select department column.
2. Under the data header, select Text to Columns option.
3. Set up the wizard and select finish.
This will separate the department and region values and the region values will be reflected in the region column we made.


7.	Duplicate values
Before moving further we should check if there are any duplicate values. Follow these steps:
1. Select all the cells using ctrl+A.
2. Under data section, choose remove duplicates option and click ok.

8.	Replacing blanks
Now we can see there are few blanks in the table. We will insert NA in those blanks. Now datasets can be large so to save time follow these steps:
1. Select all the cells.
2. Under home section, in find & select, choose go to special and choose blanks.
3. Then in the formula bar type NA and press ctrl+enter.


9.	IFERROR Function
In profit margin column, there is a formula inserted which gives error values wherever the Revenue column is NA. In order to remove the error value follow these steps:
1. Select the profit margin column. 
2. In the formula bar we will use IFERROR(value, “NA”) and press ctrl+enter.
3. This will replace the error values with NA.

10.	Formatting
Now we will format the column header to make it look presentable. We will make the column headings bold and will change the background color to blue. We can also get rid of the grid line to make it easily readable by using Alt+W+V+G. And save the file.
