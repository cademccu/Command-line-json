### Command-line-json
A utility designed as a script to turn a raw .json file into a formatted (pretty-print) version of the file, replacing it or generating a new file.

### USE

Add permisions to use as script (place in script directory or on path if you want to use everywhere):
```
chmod +x jfix
```

##### One argument use
```
jfix <FILENAME>
```
Takes one filename as an argument, writes to Python3's stdout.
##### Two argument use
```
jfix <INFILE> <OUTFILE>
```
or 
```
jfix <INFILE> -s
```
In first case, writes json  to newfile specied as second argument <OUTFILE>.
  
In second case with \"-s\", writes over <INFILE> with new indented file.
  
**USE -s WITH CAUTION!!** This could potentially fail due to permissions, or other unknown resons and the original file data could be permantley modified or lost. If this is of concern here, please use the first option or pipe the single-arg version into a file.

### OTHER
* Defaults to 4 space indentation. Change the global var INDENT_AMOUNT at the top to change this. Have not put in an option to change this yet.
