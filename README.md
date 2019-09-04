## HW_3

Create a bash for loop that extracts only the element name from each of the _.xml_ files contained in _data-shell/data/elements_ directory.  The product of the loop should be a file called _el-names.txt_  containing the element names.

*Answer: the following code finds the name element after the quotation marks, filters to get only the first file and finally it saves the element name to the text file "el-names.txt".

```
cd GEOG693/data/data-shell/data/elements
for filename in *.xml
do
cut -d '"' -f 2 $filename | head -n 1 >> el-names.txt
done
sort el-names.txt # Sort the elements in alphabetic order. 
```
