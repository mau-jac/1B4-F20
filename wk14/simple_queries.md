# Simple Queries

Queries help us find specific patterns and information that is not easily available.

Queries are commonly used for information spread across multiple tables. However, we will start with simple queries.



> 📖 For this section of the notes please refer to the following resources from GCF Global:
>
> - [Designing a Simple Query](https://edu.gcfglobal.org/en/access2016/designing-a-simple-query/1/)



## Filtering is not a Query ⚠

Beginners often confuse queries with filtering. 

There are some similarities and it is possible to "narrow" down the information we are looking for with **they are not the same thing.**

> Queries offer more flexibility and the ability to pull-in information from multiple tables. 



## Preparing a Query

Before running a query it is necessary to understand exactly what kind of data we would like to find in the database.

For example, a store might be interested in the following question:

**Which customers live in our area, are outside the city limits, and have placed an order at our store?** 

There are three pieces of information involved in answering this question:

![Identifying the data we want the query to find](https://media.gcflearnfree.org/content/56facd0b577fba179c8b6a27_03_29_2016/query_multi_planning_step1.png)

<p align="center"><a href="https://edu.gcfglobal.org/en/access2016/designing-a-multitable-query/1/"><em>Understanding the information we are looking for</em></a></p>

<br>

## Query Criteria

Building the search criteria is very similar to the criteria used for the `=SUMIF( )` and `=COUNTIF( )`  equations in Excel.

*The following criteria tables were adapted from [Query Criteria Quick Reference Guide](https://infogram.com/access-query-criteria-1g57pr4ok0zv201) from GCF Global*



### Simple criteria for all data types: 

| Criteria Name  | Write it like... | Function                                        |
| -------------- | ---------------- | ----------------------------------------------- |
| Equals         | "x"              | Searches for values equal to x                  |
| Does Not Equal | Not in ("x")     | Searches for all values except those equal to x |



### Simple criteria for text: 

| Criteria Name    | Write it like... | Function                                            |
| ---------------- | ---------------- | --------------------------------------------------- |
| Contains         | Like "\*x\*"     | Searches for all values that contain x              |
| Does Not Contain | Not like "\*x\*" | Searches for all values except those that contain x |
| Begins With      | Like "x*"        | Searches for all values beginning with x            |
| Ends With        | Like "*x"        | Searches for all values ending with x               |



### Simple criteria for numbers: 

| Criteria Name            | Write it like...    | Function                                           |
| ------------------------ | ------------------- | -------------------------------------------------- |
| Between                  | Between "x" and "y" | Searches for values in the range between x and y   |
| Less Than                | < x                 | Searches for all values smaller than x             |
| Less Than or Equal To    | <= x                | Searches for all values smaller than or equal to x |
| Greater Than             | > x                 | Searches for all values larger than x              |
| Greater Than or Equal To | >= x                | Searches for all values larger than or equal to x  |



### Simple criteria for dates: 

| Criteria Name     | Write it like...                          | Function                                                     |
| ----------------- | ----------------------------------------- | ------------------------------------------------------------ |
| Between           | Between "#mm/dd/yyyy#" and "#mm/dd/yyyy#" | Searches for dates that fall between two dates               |
| Before            | <#mm/dd/yyyy#                             | Searches for dates before a certain date                     |
| After             | >#mm/dd/yyyy#                             | Searches for dates after a certain date                      |
| Today             | =Date()                                   | Searches for all records containing today's date             |
| Days Before Today | <=Date()-x                                | Searches for all records containing dates x or more days in the past |

<br>

## Exercises

### Exercise 1

Use the Access database *Social_Sciences_Teachers.accdb* found in Teams under week 14 to complete the following tasks:

1. Create a query that returns all courses that are taught on Mondays and Wednesdays and that are worth more than 3 credits.
2. Create a query that will return all courses that start after 10am.