# filter_2col

### Installation using conda:
```conda install -c molinerislab filter_2col```

### Description
Bioinformatics and data analysis tool to filter a file based on the content of two different columns (something like grep -f).

### Usage and options:
```
filter_2col [-v] [--both-orders|b] COL_1 COL_2 filter_couple_file < input_file

-v : if indicated returns all the rows that don't match the filter (inverse filter) 
--both-orders : if indicated, the filter works indipendently of the order of <em>COL_1</em> and <em>COL_2</em> 

COL_1 : number of the first column we want the filter to use
COL_2 : number of the second column we want the filter to use
filter_couple_file : a file composed of only two columns tab-delimited 
input_file : the generic tab-delimited file we want to filter
```
returns as output the rows in ```input_file``` where the values in ```COL_1``` and ```COL_2``` match respectively with the first and the second column of the ```filter_couple_file```.

