## SED
SED command in UNIX stands for stream editor and it can perform lots of functions on file like searching, find and replace, insertion or deletion. Though most common use of SED command in UNIX is for substitution or for find and replace. By using SED you can edit files even without opening them, which is much quicker way to find and replace something in file, than first opening that file in VI Editor and then changing it.

- SED is a powerful text stream editor. Can do insertion, deletion, search and replace(substitution).
- SED command in unix supports regular expression which allows it perform complex pattern matching.


### SED Regular Expressions

- ^   start of line
- $   end of line
- .   single character
- []  match character set
- [^] exclusive Set 
- *   zero or more occurance


### POSIX Classes

Example: sed -n ‘/[[:alpha:]]/p’ posix

- [:alnum:]
- [:alpha:]
- [:digit:]
- [:blank:]
- [:lower:]
- [:upper:]
- [:punct:]
- [:space:]




### data.txt

| ID  | Name    | Salary   | Country  | Department  |
|-----|---------|----------|----------|-------------|
| 1   | Pol     | 25000    | India    | sales       |
| 2   | Bolt    | 45000    | Belgium  | clerk       |
| 3   | Loki    | 55000    | Germany  | director    |
| 4   | Hina    | 35000    | USA      | manager     |
| 5   | Ankit   | 27000    | India    | manager     |
| 6   | pawan   | 70000    | Belgium  | sales       |
| 7   | chetan  | 65000    | USA      | clerk       |
| 8   | priya   | 37000    | Germany  | director    | 
| 9   | dinesh  | 20000    | Belgium  | sales       |