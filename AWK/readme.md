awk is a scripting language, and it is helpful when working in the command line. It's also a widely used command for text processing.

When using awk, you are able to select data – one or more pieces of individual text – based on a pattern you provide.

Syntax:
awk options 'selection _criteria {action }' input-file > output-file

Options:  
-f program-file : Reads the AWK program source from the file 
                  program-file, instead of from the 
                  first command line argument.
-F fs            : Use fs for the input field separator

Built-In Variables In Awk

Awk’s built-in variables include the field variables—$1, $2, $3, and so on ($0 is the entire line) — that break a line of text into individual words or pieces called fields. 

NR: NR command keeps a current count of the number of input records. Remember that records are usually lines. If you would like each line to have a line-number count, you would use the NR built-in variable

NF: To print the last field (the last column), you can also use $NF which represents the last field in a record. 

FS: FS command contains the field separator character which is used to divide fields on the input line. The default is “white space”, meaning space and tab characters. FS can be reassigned to another character (typically in BEGIN) to change the field separator. 

RS: RS command stores the current record separator character. Since, by default, an input line is the input record, the default record separator character is a newline. 

OFS: OFS command stores the output field separator, which separates the fields when Awk prints them. The default is a blank space. Whenever print has several parameters separated with commas, it will print the value of OFS in between each parameter. 

ORS: ORS command stores the output record separator, which separates the output lines when Awk prints them. The default is a newline character. print automatically outputs the contents of ORS at the end of whatever it is given to print. 






information.txt, that contains data separated into different columns.
The file contents could look something like this:

fristName       lastName        age     city       ID

Thomas          Shelby          30      Rio        400
Omega           Night           45      Ontario    600
Wood            Tinker          54      Lisbon     N/A
Giorgos         Georgiou        35      London     300
Timmy           Turner          32      Berlin     N/A

data file

ID      Name        Salary     country       

1       ankit          25000     India        
2       Night          45000     Belgium    
3       Tinker         55000     Germany     
4       Georgiou       35000     India     

