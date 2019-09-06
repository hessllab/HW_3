## HW_3


```bash
for files in *.xml
do
cut -d '"' -f 2 $files | head -n 1 >> el-names.txt
done
```
