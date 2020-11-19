# Intro to MS Access

Spreadsheets are a great tool for analyzing data. However, they have the following limitations:

- Data in tables are not directly linked or associated to other tables
- Entering and retrieving data is not user friendly
- It is difficult to enforce that data is entered correctly (everything is possible: numbers vs words vs dates)



**In practice, the information we are looking for is often distributed in amongst multiple tables.**



> 📖 For this section of the notes please refer to the following resources from GCF Global:
>
> - [Introduction to Objects](https://edu.gcfglobal.org/en/access2016/introduction-to-objects/1/)
> - [Managing Databases and Objects](https://edu.gcfglobal.org/en/access2016/managing-databases-and-objects/1/)



For example, consider the following Home Depot invoice:

<br>

![Example of a home depot invoice](https://image.slidesharecdn.com/invoice-august32018materialstuffboughtfortherepairs208westhavendrive78746-180803195223/95/invoice-august-3-2018-material-stuff-bought-for-the-repairs-208-westhaven-drive-78746-1-638.jpg?cb=1533325952)

<p align="center"><a href="https://destemperados.blogspot.com/2018/12/home-depot-invoice.html"><em>Example of a HomeDepot invoice</em></a></p>

<br>

A typical  store needs to keep track of the following information:

<br>

![Four pages each with the fields required for different types of data](https://fmhelp.filemaker.com/help/16/fmp/en/FMP_Help/images/relational.07.12.5.png)

<p align="center"><a href="https://fmhelp.filemaker.com/help/16/fmp/en/index.html#page/FMP_Help/planning-databases.html"><em>Common information that needs to be tracked by a store</em></a></p>

<br>

Each individual table illustrated above could be stored in an Excel sheet. However, there is a relationship between each one of those tables that also needs to be recorded.

Some fields in one table are coming directly from another table. Other fields are repeated in multiple tabled which creates data duplication and are hard to keep up to date.

<br>

![Showing relationships between multiple tables and removing duplicated data](https://fmhelp.filemaker.com/help/16/fmp/en/FMP_Help/images/relational.07.12.8.png)

<p align="center"><a href="https://fmhelp.filemaker.com/help/16/fmp/en/index.html#page/FMP_Help/planning-databases.html"><em>Showing relationship between key data and removing duplication</em></a></p>

<br>

> Databases are a collection of linked tables. They are designed so that:
>
> - Information is accurate and organized
> - No redundant or duplicate information
> - It’s easy to find information



## Overview: the four objects of an Access database

MS Access databases are organized in the following objects:

<br>

**Tables**: Where the records (data) are stored. Similar to Excel.

**Forms**: Visual “guide” for entering, modifying and viewing records

**Queries**: Searching and compiling data from tables

**Reports**: Visually presenting data in a easily readable and printable way

<br>

![The four objects of a database](https://lh5.googleusercontent.com/VNSuSpcq-oYKkvjQ0i2pwdRXW3V061q_QJU0x9s95U1jxAPqzdtzf7V2Y_z0Nx4R6kH4MPVN-6IXTzytUYN6EFtsoIIhTcOCtuQAPLoNtso32HwjiAxKCfyybHZd5i4FA9UY5KMqnXE)



### Tables

Tables store the data in a way that is similar to Excel.

There are some minor differences in terminology:

<br>

![Example of Access table](https://lh5.googleusercontent.com/kOMTS0p0IUzOQ7IaS87cT58k5qbBDCieGCpt4VYT0TmjwkjbYtclQ3NffdFJ3LaezY4vOzlJbh-aedWiPSp8YJjl1b68wUTZ1Vgy6v4ghtCMavBZCfjsl2YJRQFSjGL3CaOqJy9LjuU)

<br>

1. **Records (rows)**: contains specific data, like information about a particular employee or a product.
2. **Fields (columns):** contains data about one aspect of the table subject, such as first name or e-mail address.
3. **Field value (cell)**: Each record has a field value. For example, Contoso, Ltd. or someone@example.com.



> Every **value** within a **field** is of the same **type**. There are different types of data (date vs number vs text).
>
> A **record** is a unit of information. Every cell in a given row is part of the **same record**.
>
> The **ID number** for a record refers to all information contained on that row. ID numbers are **unique** and should not be modified.



### Forms

Forms offers us a more user-friendly way of manipulating the data in the tables.

<br>

![Example of Access form](https://lh6.googleusercontent.com/sNWanHX34vicipdteHm5E9J-P-IRbFyBDEZe4FQ0sr_Up6Er0HFHa2WtWCFilEPrFfZ7Yd54UszXcIxdM5AtQdnUVxBghavu9CGJ12BRg9owJQtCoAVV_oZm5tgohQBvrUGJLANPP50)

<br>

It’s the same **data from the tables** but in a **different visual format**.

It makes entering and modifying data easier and it allows users to enter data into multiple tables at once.

### Queries

Since most tables are linked via different relationships, **queries** allows us to retrieve **specific data** from one of more tables.

> Queries need to be structured in order to ask specific questions.

![img](https://lh5.googleusercontent.com/dFIJJ4WM2O0CZ-YAWdxxxIJ0J1uIjQt_qRjIemepQktryWzybZC29cEQw7CppvLRFG-iw_F84RRwXKbUYUccUbOGbN1QWn5mHCGu6EgXeJTlJVA1-02Oz-8UNeWMRyEtvS7xrGOk_1Q)![image-20201117144932779](assets/image-20201117144932779.png)

For example:

*“What is the name, email and address of all customers who ordered product X in the last 3 months ?”*

### Reports

Reports present data from any table or query. in an **easy-to-read** (or print) format.

It is possible to customize reports in order to make it visually appealing.

<br>

![Example of a Report in MS Access](https://lh4.googleusercontent.com/ECLBCbp7ZyoZ6DVTZt5eR1BLcCXKcO74-qOCq-4WW25I3_Kf21yaUZ2Rx5F29auciBQBWwFzEOlzpbIQ8UyGgw52Bl9WFnCBaq8QtAN48QbdVqTjxUbqRmvyIDBSOnhqw9kNwstVGBQ)