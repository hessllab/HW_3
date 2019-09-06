## HW_3

Create a bash for loop that extracts only the element name from each of the _.xml_ files contained in _data-shell/data/elements_ directory.  The product of the loop should be a file called _el-names.txt_  containing the element names.

*Answer: the following code looks for the element name within each file that has a `.xml` extension. After it has found the name element after the quotation marks, the code filters the output to only get the first line. Finally, it saves the element name to the text file "el-names.txt" As the loop progresses it will appends the next value to el-names.txt.* 

```
cd GEOG693/data/data-shell/data/elements
for filename in *.xml
do
    cut -d '"' -f 2 $filename | head -n 1 >> el-names.txt #reverse these two for faster processing time
done
sort el-names.txt # Sort the elements in alphabetic order. #nice addition.
```
