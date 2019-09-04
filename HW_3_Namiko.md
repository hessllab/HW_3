```  
for filename in *xml
do
echo $filename
cut -d \" -f 2 $filename | head -n 1 >> el-names.txt
done
```  