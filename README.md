# SQL-Server-Date-Functions

# Introduction to SQL Server Date and Time Functions.

SQL Server has varities of Date and Time functions which are widely used for Data/Date Manipulation.
This tutorial will help to understand some of the most used Date and Time functions.

# SQL Server SYSDATETIME, SYSDATETIMEOFFSET and SYSUTCDATETIME Functions:
-> SYSDATETIME – returns the date and time of the machine the SQL Server is running on
-> SYSDATETIMEOFFSET – returns the date and time of the machine the SQL Server is running on plus the offset from UTC
-> SYSUTCDATETIME - returns the date and time of the machine the SQL Server is running on as UTC

![image](https://user-images.githubusercontent.com/122970222/213415402-3f834b6c-8270-4910-aa83-fb1cf7205b85.png)

# SQL Server CURRENT_TIMESTAMP, GETDATE() and GETUTCDATE() Functions
-> CURRENT_TIMESTAMP - returns the date and time of the machine the SQL Server is running on
-> GETDATE() - returns the date and time of the machine the SQL Server is running on
-> GETUTCDATE() - returns the date and time of the machine the SQL Server is running on as UTC

![image](https://user-images.githubusercontent.com/122970222/213415772-e0c72c7b-e52d-475a-92a4-1eb5ace53b9b.png)

SELECT DATENAME(YEAR, GETDATE())        AS 'Year';        
SELECT DATENAME(QUARTER, GETDATE())     AS 'Quarter';     
SELECT DATENAME(MONTH, GETDATE())       AS 'Month Name';       
SELECT DATENAME(DAYOFYEAR, GETDATE())   AS 'DayOfYear';   
SELECT DATENAME(DAY, GETDATE())         AS 'Day';         
SELECT DATENAME(WEEK, GETDATE())        AS 'Week';        
SELECT DATENAME(WEEKDAY, GETDATE())     AS 'Day of the Week';     
SELECT DATENAME(HOUR, GETDATE())        AS 'Hour';        
SELECT DATENAME(MINUTE, GETDATE())      AS 'Minute';      
SELECT DATENAME(SECOND, GETDATE())      AS 'Second';      
SELECT DATENAME(MILLISECOND, GETDATE()) AS 'MilliSecond'; 
SELECT DATENAME(MICROSECOND, GETDATE()) AS 'MicroSecond'; 
SELECT DATENAME(NANOSECOND, GETDATE())  AS 'NanoSecond';  
SELECT DATENAME(ISO_WEEK, GETDATE())    AS 'Week';    

SQL Server T-SQL Syntax	Date Function	Result
SELECT DATENAME(YEAR, GETDATE()) AS 'Year';	Year	2019
SELECT DATENAME(QUARTER, GETDATE()) AS 'Quarter';	Quarter	1
SELECT DATENAME(MONTH, GETDATE()) AS 'Month';	Month	March
SELECT DATENAME(DAYOFYEAR, GETDATE()) AS 'DayOfYear';	DayOfYear	67
SELECT DATENAME(DAY, GETDATE()) AS 'Day';	Day	8
SELECT DATENAME(WEEK, GETDATE()) AS 'Week';	Week	10
SELECT DATENAME(WEEKDAY, GETDATE()) AS 'WeekDay';	WeekDay	Friday
SELECT DATENAME(HOUR, GETDATE()) AS 'Hour';	Hour	11
SELECT DATENAME(MINUTE, GETDATE()) AS 'Minute';	Minute	25
SELECT DATENAME(SECOND, GETDATE()) AS 'Second';	Second	44
SELECT DATENAME(MILLISECOND, GETDATE()) AS 'MilliSecond';	MilliSecond	426
SELECT DATENAME(MICROSECOND, GETDATE()) AS 'MicroSecond';	MicroSecond	426666
SELECT DATENAME(NANOSECOND, GETDATE()) AS 'NanoSecond';	NanoSecond	426666666
SELECT DATENAME(ISO_WEEK, GETDATE()) AS 'Week';	Week	10
![image](https://user-images.githubusercontent.com/122970222/213416896-da932858-5494-4c1a-a450-f7669b9331a6.png)
