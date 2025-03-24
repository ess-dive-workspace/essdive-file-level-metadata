# CSV Data Dictionary

## Instructions

1. Create a CSV data dictionary using the [CSV\_dd\_template](CSV_dd_template.csv).  You can create either:  
&nbsp;&nbsp;&nbsp;a. One data dictionary for each data file or  
&nbsp;&nbsp;&nbsp;b. One data dictionary representing all data files in your dataset    

2. See the [CSV\_dd\_quick\_guide](csv_dd_quick_guide.md) for more details about completing the template  
3. Enter a new row in the data dictionary for each column/row name in your data matrix  
&nbsp;&nbsp;&nbsp;a. Use "\*" wildcard when the description applies to multiple column/row names  
&nbsp;&nbsp;&nbsp;b. For example - if the same description applies to all spectra data column names in the data file(s)   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i. one row in the data dictionary can refer to "wave_\*\" and this definition will be understood to apply to multiple column names within a data sheet     
            
4. View an example [CSV\_dd\_example](csv_dd_example.md)  

5. Save the CSV\_dd template following the [CSV Reporting Format guidance](https://github.com/ess-dive-workspace/essdive-csv-structure) with the filename "dd.csv" or "\*\_dd.csv". Alternatively you may choose to name you data dictionary:  
&nbsp;&nbsp;&nbsp;a. With the same name as the associated data file, but include '\_dd.csv' at the end of the file name  
&nbsp;&nbsp;&nbsp;b. Create a unique filename for your data dictionary  
&nbsp;&nbsp;&nbsp;c. Incorporate a wildcard into the filename if data dictionary applies to multiple data files (for example - "soil_cores_\*\_dd.csv")  

**Contents of the CSV\_dd**

For each variable provide the following:

* Column or Row Name  
* Unit  
* Definition  
* Column or Row Long Name
* Data Type
* Missing Value Code 

**Notes**  

Following the recommended format and structure of the CSV Reporting Format will facilitate File Level Metadata extraction of some fields using the [File Level Metadata Extractor](https://code.ornl.gov/ngee-arctic/ess-dive-meta).

