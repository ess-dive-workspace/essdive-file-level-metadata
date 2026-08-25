# Instructions
The File Level Metadata (FLMD) file is used to describe files contained within a single dataset.

## Resources
- [Instructions](/file_level_metadata_flmd/flmd_instructions.md)
- [Term Guide](/file_level_metadata_flmd/term_guide.md) and [Controlled Vocabulary](/file_level_metadata_flmd/controlled_vocabulary.md)
- [Template](/file_level_metadata_flmd/template_flmd.csv)
- [Examples](/file_level_metadata_flmd/examples/)

## Format
- Comma delimited file (.csv) following the [CSV reporting format](https://github.com/ess-dive-workspace/essdive-csv-structure)
- FLMD terms in the first row are the file headers (horizontal orientation)
- File name is “flmd.csv” or ends with “_flmd.csv”

## Minimum requirements
- List and define all files.
    - Include file extensions (e.g., .csv, .pdf, .txt) in the filename
- Wildcards can be used. See details in Additional Guidance.
- Provide a short file description
- When publishing an FLMD on ESS-DIVE, include the keyword "ESS-DIVE File Level Metadata Reporting Format" within the dataset metadata Keywords section.

## Additional Guidance
- Wildcards can be used within the file_name term when there are multiple files with similar file names and the same file description.
    - Example: For files named temp_plot1.csv and temp_plot2.csv that contain the same type of temperature data, enter temp_plot*.csv in the FLMD file_name term and provide a single description.
- If you have organized the data files in folders, it is recommended to enter the full path of the file.
    - Example: /data/site2/temperature/temp_plot*.csv
- Header rows and row/column name position details:
    - If a data file has additional header rows/columns before or after the row/column names, be sure to provide entries for the “header_rows” and “column_or_row_name_position” fields. The inclusion of these fields will be required for parsing the files.
    - If you have any header rows commented out with a hash (#), these will be skipped during parsing. Do not include any commented-out headers in the “header_rows” or “column_or_row_name_position” counts.
    - Review the following examples for use of the “header_rows” and “column_or_row_name_position” fields: example 1, example 2, example 3.
    - Other reporting formats that have specific FLMD requirements must be followed if the other reporting format is used within the data package. For example, some data specific reporting formats require extensions to the data dictionary files and must be separated from a general data dictionary file(s).
