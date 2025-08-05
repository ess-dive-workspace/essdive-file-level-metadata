# Instructions for ESS-DIVE File Level Metadata Reporting Format

1. Create file-level metadata for each data set using the provided template.  
&nbsp;&nbsp;&nbsp;a. Start new row for each file and include all files.  
&nbsp;&nbsp;&nbsp;b. Use "\*" wildcard when an FLMD entry applies to multiple files with similar naming conventions.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; For example - the same FLMD row information applies to all soil core files in this data package - "soil\_cores\_\*\.csv"  
2. Follow the instructions in the [FLMD quick guide](flmd_quick_guide.md). 
3. Use the [FLMD template](flmd_template.csv).  
4. Save the FLMD template as a CSV. Name the flmd file "flmd.csv" or you can include a prefix in the form of "\*\_flmd.csv".  
5. For CSV data files, create a [CSV Data Dictionary](CSV_dd/) to describe the fields and other attributes of your CSV data file. The data dictionary file should be listed in your FLMD file (described in step 1). 
6. We recommend including the FLMD outside of any zip files for easy identification, but you may also include it in the zip file.
7. If submitting your dataset to ESS-DIVE, include the keyword **ESS-DIVE File Level Metadata Reporting Format** in the package-level metadata.

**Notes**

* Fields common to ESS-DIVE Package Level Metadata are consistent in format structure
* If a data file has multiple header rows and/or additional header rows/columns before or after the row/column names, be sure to provide entries for the “header_rows” and “column_or_row_name_position” fields. The inclusion of these fields will be required for parsing the files.
* If you have any header rows commented out with a hash (#), these should be skipped during parsing. Do not include any commented-out headers in the “header_rows”  or “column_or_row_name_position” counts.
* Review the following examples for use of the “header_rows” and “column_or_row_name_position” fields: [example 1](flmd_header_rows_example_1.png), [example 2](flmd_header_rows_example_2.png), [example 3](flmd_header_rows_example_3.png).   

**Contents of the Elements**

* file_name 
* file_description
* standard  
* file_version
* data_orientation  
* header_rows
* column_or_row_name_position
* notes

