# Quick guide for ESS-DIVE File Level Metadata Reporting Format

Elements of the reporting format:  
* [file_name](#file-name)  
* [file_description](#file-description)  
* [standard](#standard)
* [file_version](#file-version)
* [data_orientation](#data-orientation)
* [header_rows](#header-rows)
* [column_or_row_name_position](#column-or-row-name-position)
* [notes](#notes)  

---  

### File Name  
|Metadata Element|file_name|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Name of the file|
|Reporting Format Definition|Provide the name of the associated file. File names should be unique and be as descriptive as possible about the file contents. Use only letters (e.g. CamelCase), numbers, and underscores. Do not include spaces. Hyphens allowed but not preferred. Use "\*" wildcard when the FLMD applies to multiple files. For example - the same FLMD applies to all soil core files in this data package - "soil&#95;cores&#95;\*\.csv"|
|Required, Recommended or Optional|required|
|Format||

### File Description
|Metadata Element|file_description|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|A brief description of the file|
|Reporting Format Definition|A brief description (minimum of 10 characters) of the file and what distinguishes this file from other files in the data package. Include information about the type of data (images, observations, experimental, etc.) |
|Required, Recommended or Optional|required|
|Format||

### Standard  
|Metadata Element|standard|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|standard applied to the data file.|
|Reporting Format Definition|Identify if an ESS-DIVE Reporting Format or any other data or metadata standard was applied to the data file. Standard names for the ESS-DIVE reporting formats are available in the [Standard FLMD Term List](RF_FLMD_Standard_Terms.csv).| 
|Required, Recommended or Optional|strongly recommended|
|Format||


### File Version  
|Metadata Element|file_version|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|The version of the file.|
|Reporting Format Definition|This is the version of the data file being described in the FLMD. The data file version is assigned by the data provider and not by the system. This would change if the data file is updated after the data package is published. Changes should be explained in the Notes field.|
|Required, Recommended or Optional|optional|
|Format||

### Data Orientation  
|Metadata Element|data_orientation|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Orientation of tabular data|
|Reporting Format Definition|Describe how the data are organized within the data matrix. Choose between "horizontal" (i.e., data are organized in rows) or "vertical" (i.e., data are organized in columns).|
|Required, Recommended or Optional|optional|
|Format||  

### Header Rows
|Metadata Element|header_rows|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Number of header rows.|
|Reporting Format Definition|Provide the total number of header rows before the start of the first data row, including the column header or row name (except for any commented-out headers). This field is marked as optional, but is required if any data files have more than one header row. Review the following examples for use of the “header_rows” field: [example 1](flmd_header_rows_example_1.png), [example 2](flmd_header_rows_example_2.png), [example 3](flmd_header_rows_example_3.png).|
|Required, Recommended or Optional|optional, **required if dataset has multiple header rows**|
|Format|number|

### Column or Row Name Position
|Metadata Element|column_or_row_name_position|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Position of the column or row that contains the column or row names.|
|Reporting Format Definition|Provide the row or column number that contains the header names. This field is not required if there are no rows or columns before the row/column names. If not included, it will be assumed that header names are in row 1 (horizontal orientation) or column 1 (vertical orientation). If there are rows/columns after the header names, note these using the header_rows field. Review the following examples for use of the “column_or_row_name_position” field: [example 1](flmd_header_rows_example_1.png), [example 2](flmd_header_rows_example_2.png), [example 3](flmd_header_rows_example_3.png).|
|Required, Recommended or Optional|optional, **required if rows or columns are provided before the row/column names**|
|Format|number|

### Notes  
|Metadata Element|notes|
|:----------------------------------------------------|:----------------------------------------------------|
|Reporting Format Statement|Any information the provider would like to add.|
|Reporting Format Definition|Information provided would be data file specific. Details may include details on data file versioning, reporting format, software requirements, data quality, etc.|
|Required, Recommended or Optional|optional|
|Format||
