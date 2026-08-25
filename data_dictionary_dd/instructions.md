# Instructions
The data dictionary (DD) file is used to describe column or row name headers within CSV file(s). 

You have the following options when providing data dictionary file(s) for your dataset:
- **1:1** – One data dictionary for each data file, or
- **1:All** – One data dictionary representing all data files in your dataset, or
- **1:Multiple** – Multiple data dictionaries representing a subset of data files in your dataset.

Other reporting formats may have additional or other data dictionary requirements that must be followed for compliance with those reporting formats.

## Resources
- [Term Guide](/data_dictionary_dd/term_guide.md) and [Controlled Vocabulary](/data_dictionary_dd/controlled_vocabulary.md)
- [Template](/data_dictionary_dd/template_dd.csv)
- [Examples](/data_dictionary_dd/examples/)

## Format
- Comma delimited file (.csv) following the [CSV reporting format](https://github.com/ess-dive-workspace/essdive-csv-structure)
- Data dictionary terms in the first row are the file headers (horizontal orientation)
- File name is “dd.csv” or ends with “_dd.csv”

## Minimum requirements
- List and define all column or row headers in the CSV file, exactly as they appear
- Specify the unit associated with the column or row header
- Provide a short header description
- When publishing an FLMD on ESS-DIVE, include the following
    - Include the keyword "ESS-DIVE File Level Metadata Reporting Format" within the dataset metadata Keywords section.

## Additional Guidance
- Within a data dictionary file, the column_or_row_name values must be unique. If the same header name is used in multiple CSV files and have different definition, units, etc, separate data dictionary files must be provided for each specification of the header name.
- The data dictionary can also be used to describe other tabular formats, but these other formats will not be parsed by ESS-DIVE.
- Other reporting formats that have specific data dictionary requirements must be followed if the other reporting format is used within the data package.
