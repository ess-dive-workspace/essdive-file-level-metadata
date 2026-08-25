# Term Guide
The file level metadata terms are defined below, including whether that term is required, a brief definition, formatting requirements, an example, and additional guidance. 

### Terms of the reporting format:
* [file_name](#file_name)  
* [file_description](#file_description)  
* [standard](#standard)
* [data_dictionary_file_name](#data_dictionary_file_name)
* [file_version](#file_version)
* [data_orientation](#data_orientation)
* [header_rows](#header_rows)
* [column_or_row_name_position](#column_or_row_name_position)
* [notes](#notes)  

---  
### file_name
|term|`file_name`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|required|
|format|free text|
|definition|Provide the name of the file. File names should be unique and as descriptive as possible about the file contents. Use only letters (e.g. CamelCase), numbers, and underscores. Do not include spaces. Hyphens allowed but not preferred. Use "\*" wildcard when the file name applies to multiple files. For example - the same file name applies to soil core files in the data package - "soil_cores_*.csv"|
|example|measurements.csv|
|additional guidance|If the files are organized into folders, it is recommended to include the full path, for example: /data/site2/temperature/temp_plot*.csv <br><br> Do not define the zip file name only within your File Level Metadata file.|

### file_description
|term|`file_description`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|required|
|format|free text|
|definition|A brief description (minimum of 10 characters) of the file and what distinguishes this file from other files in the data package. Include information about the type of data (images, observations, experimental, etc.)|
|example|Geochemistry data measurements, including anions and cations, for 2025-06-08 to 2026-01-02.|
|additional guidance|N/A|

### standard
|term|`standard`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|recommended|
|format|[Controlled vocabulary](https://github.com/ess-dive-workspace/essdive-file-level-metadata/blob/release-v1.2.0/file_level_metadata_flmd/controlled_vocabulary.md#standard)|
|definition|Identify if an ESS-DIVE Reporting Format or any other data or metadata standard was applied to the data file.|
|example|ESS-DIVE FLMD v1|
|additional guidance|Only one standard should be entered per file. <br><br> If you have a file that follows multiple reporting formats (e.g., Sample Data - Full and CSV guidelines reporting formats), provide the reporting format standard term that the file should be parsed as. For example, for files governed by the Sample Data - Full reporting format, the standard term should be “ESS-DIVE Sample Data - Full Reporting Format v1”, **not** “ESS-DIVE CSV File Formatting Guidelines Reporting Format”. <br><br> The version number within the standard term contains only the major version number. If a reporting format has minor and patch versions, these should not be provided within the standard term.|

### data_dictionary_file_name
|term|`data_dictionary_file_name`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|optional|
|format|text; contains “dd.csv"|
|definition|The file name of the data dictionary that corresponds to the provided “file_name” entry. The file name must be “dd.csv” or end with “_dd.csv”.|
|example|measurements_dd.csv|
|additional guidance|This term is required for data files that are csv or other tabular format and that have an associated data dictionary file. Other reporting formats may require this term be provided for certain additional file types. <br><br> Wildcards are not permitted within the `data_dictionary_file_name`.|

### file_version
|term|`file_version`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|optional|
|format|free text|
|definition|This is the version of the data file. The data file version is assigned by the data provider and not by the system. The version should change if the data file is updated after the data package is published or re-published. Explain the changes in the `notes` term.|
|example|version 1|
|additional guidance|N/A|

### data_orientation
|term|`data_orientation`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|optional|
|format|[Controlled vocabulary](https://github.com/ess-dive-workspace/essdive-file-level-metadata/blob/release-v1.2.0/file_level_metadata_flmd/controlled_vocabulary.md#data_orientation)|
|definition|Describe how the data are organized within the data matrix. Choose between "horizontal" (i.e., data are organized in rows with column headers) or "vertical" (i.e., data are organized in columns with row headers).|
|example|horizontal|
|additional guidance|N/A|

### header_rows
|term|`header_rows`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|Required conditionally for files with more than one header row|
|format|integer|
|definition|Provide the total number of header rows before the start of the first data row, including the column header or row name. Do not include commented-out (i.e., column/rows that begin with a hash (#)) in the header_rows count. This term is required if any data files have more than one header row.|
|example|1|
|additional guidance|N/A|

### column_or_row_name_position
|term|`column_or_row_name_position`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|Required conditionally for files with rows or columns before the header names|
|format|integer|
|definition|Provide the row or column number that contains the header names. This term is required if there are rows or columns before the header names. If not provided,  the header names are assumed to be in row 1 (horizontal orientation) or column 1 (vertical orientation). Do not include commented-out (i.e., column/rows that begin with a hash (#)) in the column_or_row_name_position count.|
|example|1|
|additional guidance|N/A|

### notes
|term|`notes`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|optional|
|format|free text|
|definition|Additional information for the data file. Information may include details on data file versioning, reporting format, software requirements, data quality, etc.|
|example|N/A|
|additional guidance|N/A|
