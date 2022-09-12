# filter_2col
a tool to filter a file on the content of two different columns (something like grep -f)

## how to use
synatx:
<p align="center">
<em> filter_2col [-v] [--both-orders|b] COL_1 COL_2 filter_couple_file < input_file </em>
<p>

returns as output the rows in <em>input_file</em> where the values in <em>COL_1</em> and <em>COL_2</em> match respectively with the first and the second column of the <em>filter_couple_file</em>
* <em>-v</em> : if indicated returns all the rows that don't match the filter (inverse filter) 
* <em>--both-orders</em> : if indicated the filter works indipendently of the order of <em>COL_1</em> and <em>COL_2</em> 
* <em>COL_1</em> : number of the first column we want the filter to use
* <em>COL_2</em> : number of the second column we want the filter to use
* <em>filter_couple_file</em> : a file composed of only two columns tab-delimited 
* <em>input_file</em> : the generic tab-delimited file we want to filter
