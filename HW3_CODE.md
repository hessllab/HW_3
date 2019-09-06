# Homework 3 Code
For this assignment, the goal was to create a loop to extract only one variable from a list of files (only .xml files) in this case. 
Once the variable was extracted from each file in the list, the loop placed each varialbe in a text file. In this example, the varialbe 
was the element name.


## Code
```
for filename in *.xml
do
cut -d \" -f 2 $filename | head -n 1 >> el-names.txt
done
```

## Output Example

```
Actinium
Silver
Aluminum
Americium
Argon
Arsenic
Astatine
Gold
Boron
Barium
Beryllium
Bismuth
Berkelium
Bromine
Carbon
Calcium
Cadmium
Cerium
Californium
Chlorine
Curium
Cobalt
```

