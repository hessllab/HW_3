## Zack - HW3

Create a bash for loop that extracts only the element name from each of the _.xml_ files contained in _data-shell/data/elements_ directory.  The product of the loop should be a file called _el-names.txt_  containing the element names.

### Solution:
```  
for filename in *.xml
    do head -n 1  $filename | cut -d '"' -f 2
done  
```
