csv2sql
=======

## Introduction
A very simple PHP script that converts a CSV file to a SQL dump. The script expects the CSV file to be in a proper format that is readable to PHP's `fgetcsv`.

All values should be enclosed in double quotes (") and seperated by commas (,). Furtheremore, the first line of your file is used for the names of the rows.

Here's a simple example of a proper CSV file:

    "id", "book", "author"
    "1", "1984", "George Orwell"
    "2", "Hamlet", "Shakespeare"

## Usage
1. Make this command executable


    chmod +x ./csv2sql
    

2. Use it from the commandline like this


    csv2sql file.csv table_name
    

The output will go to stdout, so to write it to a file do something like this:

    csv2sql file.csv table_name > import.sql
    

## Credits
Written by [Hay Kranen](http://www.haykranen.nl) ([@hayify](http://www.twitter.com/hayify)).

Patches and comments welcome on [Github](https://github.com/hay/csv2sql)
