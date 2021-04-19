# How to process csv file in python

Version: 0.1

CSV is a very common file format to store and transfer data. We can treat CSV as table-like object, the same as relational database table, and Microsoft Excel.

CSV has some features other table-like data processing tools don't have.

- You can open it with plain old text editor.
- Because it's a text file, you can easily treat it as a content transfering media, and it's easy to debug.
- You can track the change using Version Control Systems like Git.

## Python and CSV

Python provides a standard library for CSV processing. But it's a bit low-level.

## A protocol for CSV

Here I provided protocol for CSV file used in data analysis.

- CSV file should be treated as table
- CSV file should have table header, so you can track the meaning of data in the future
- CSV file should be sorted by a key, so you can track changes in GIT

### Additional issues

Many CSV processor tools like Microsoft Excel, Python Pandas assume the data type in a column. This feature causes many problems than the problems it solves.


## Compare CSV with DB software

### CSV and Relational data

- flexible schema
- You can use csv processor to modify schema for
    - more easily generate figures in R, the issue of R is it's syntax.

### CSV and NoSQL

- more solid schema
