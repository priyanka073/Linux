## AWK

awk is a scripting language, and it is helpful when working in the command line. It's also a widely used command for text processing.

When using awk, you are able to select data – one or more pieces of individual text – based on a pattern you provide.
It acts as a filter in Linux. It is also referred as gawk (GNU awk) In Linux.

It is one of the most widely used tools for the programmer, as they write the scaled-down effective program in the form of a statement to define the text patterns and designs.

## How is it named as AWK?
This command is named by using the first letter of the name of three people who wrote the original version of this command in 1977. Their names are Alfred Aho, Peter Weinberger, and Brian Kernighan and they were from AT & T Bell Laboratories.


## Features of AWK command
Various features of the Awk command are as follows:

It scans a file line by line.
It splits a file into multiple fields.
It compares the input text or a segment of a text file.
It performs various actions on a file like searching a specified text and more.
It formats the output lines.
It performs arithmetic and string operations.
It applies the conditions and loops on output.
It transforms the files and data on a specified structure.
It produces the format reports.


## Syntax:
awk options 'selection _criteria {action }' input-file > output-file


## Options:  
- -f program-file : Reads the AWK program source from the file 
                  program-file, instead of from the 
                  first command line argument.
- -F fs            : Use fs for the input field separator


 ## Built-In Variables In Awk

Awk’s built-in variables include the field variables—$1, $2, $3, and so on ($0 is the entire line) — that break a line of text into individual words or pieces called fields. 

- NR: NR command keeps a current count of the number of input records. Remember that records are usually lines. The awk command performs action once for each line. These lines are said as records.

- NF: To print the last field (the last column), you can also use $NF which represents the last field in a record. 

- FS: It is used to create a field separator character to divide fields into the input lines.

- RS: RS command stores the current record separator character. Since, by default, an input line is the input record, the default record separator character is a newline. 

- OFS: It is used to store the output field separator. It separates the output fields.

- ORS: It is used to store the output record separator. It separates the output records. It prints the content of the ORS command automatically.



### employee.txt

| Name   | Post     | Department | Salary | ID  |
|--------|----------|------------|--------|-----|
|        |          |            |        |     |
| ajay   | manager  | account    | 45000  | 400 |
| sunil  | clerk    | account    | 25000  | N/A |
| varun  | manager  | sales      | 50000  | 600 |
| amit   | manager  | account    | 47000  | 400 |
| tarun  | peon     | sales      | 15000  | N/A |
| deepak | clerk    | sales      | 23000  | 400 |
| sunil  | peon     | sales      | 13000  | 500 |
| satvik | director | purchase   | 80000  | 300 |





