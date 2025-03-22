# ESS-DIVE File Level Metadata Reporting Format v1.1.1

File level metadata provides granular information at the data file level to enable comparison of data files within a data set and the ability to search for and locate files across the data collection. The recommended file level metadata \(FLMD\) schema will describe the contents, scope, and structure of the data file within the ESS-DIVE repository. This metadata is fully consistent with and augments the metadata collected to describe each data set.

## Getting started

Instructions for how to use this reporting format:

* [File level metadata reporting format instructions](flmd_instructions.md)

Other documents:

* [File level metadata quick guide](flmd_quick_guide.md)   
* [File level metadata template](flmd_template.csv) 

          - [Includes example template](flmd_template_example.csv)  

* CSV Data Dictionary  

          - Includes [instructions](CSV_dd/README.md), [template](CSV_dd/CSV_dd_template.csv), and [example](CSV_dd/csv_dd_example.md)

---  
## Updates in v1.1.1
In March 2025, a patch version of the File Level Metadata reporting format was made to improve the overall experience with the associated reporting format documentation. For more specific details, review the release notes for v1.1.1.

## Updates in v1.1.0
The File Level Metadata reporting format was updated in April of 2024 to address usability challenges and feedback from early adopters. All templates and instructions have been updated accordingly. These changes are backwards compatible and parsable by the ESS-DIVE Fusion Database. The revisions are as follows:

* Removing excess optional fields
  * In an effort to streamline the file level metadata file, we have removed the following optional fields from the documentation: _UTC offset, Contact, Date Start / Date End, Coordinates, Latitude / Longitude_
  * The optional field _missing value codes_, which can be used to declare the codes representing missing values, has been added to the data dictionary file so that it can be used at the variable level.
* Adding variables to allow for better handling of header rows that do not contain variable information
  * The optional variables _header rows_ and _column or row name position_ can be used to provide the number of rows that occur either before or after variable names. Including these variables is important to increase the parsability of files with additional metadata rows that precede data entries. For more instruction on how to use these variables, please refer to our updated [File level metadata reporting format instructions](flmd_instructions.md).
* Adding standard reporting format keywords to be used in the _standard_ field
  * The optional _standard_ keyword in the file level metadata file can be used to declare a standard or format that a file follows. If a file uses an ESS-DIVE reporting format, we now recommend using the corresponding [FLMD standard name](RF_FLMD_Standard_Terms.csv).
* Standardizing variable naming convention to snake case
  * The original FLMD field names used both underscores and capitalizations and did not follow a specific naming convention. In v1.1.0, we have updated the formatting of field names to follow snake case guidelines, for example File_Name -> file_name; Column_or_Row_Name -> column_or_row_name. No spelling or underscore placement has been revised. Our goal is to increase consistency and harmonize across the reporting formats. While templates and instructions have been updated to reflect this convention change, the original capitalization will still be accepted as long as spelling and use of underscores is consistent. 

## How to contribute  
This ESS-DIVE File Level Metadata reporting format is evolving and growing to meet the needs of researchers. Feedback and new contributions are welcome. If you would like to suggest a change to the file level metadata reporting format please submit a [GitHub issue](https://github.com/ess-dive-workspace/essdive-file-level-metadata/issues/new/choose) using one of the templates we provide.

If you have any questions about this reporting format, you can also directly email ESS-DIVE support at ess-dive-support@lbl.gov.  

Our issue templates were based on those used by Darwin Core.  
Darwin Core maintenance group, Biodiversity Information Standards \(TDWG\) \(2014\). Darwin Core. Zenodo. [https://doi.org/10.5281/zenodo.592792](https://doi.org/10.5281/zenodo.592792)

## Copyright information

This repository content is license for use under the [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/)

## Funding and acknowledgements

Funding for the development of ESS-DIVE File Level Metadata Reporting Format was provided by the U.S. Department of Energy, Office of Science, Office of Biological and Environmental Research, Climate and Environmental Science Division, Data Management program under contract number DE-AC02-05CH11231.

## Recommended citation

Velliquette, T., Welch, J., Crow, M., Devarakonda, R., Heinz, S., Crystal-Ornelas, R. (2021). ESS-DIVE Reporting Format for File-level Metadata. Environmental Systems Science Data Infrastructure for a Virtual Ecosystem (ESS-DIVE), ESS-DIVE Repository. https://doi.org/10.15485/1734840

## Related reference

McNelis, J., Crow, M., and Devarakonda, R., ESS-DIVE File Level Metadata Extractor. Computer Software. https://code.ornl.gov/ngee-arctic/ess-dive-meta. 01 Oct. 2020. Web. doi:10.11578/dc.20201103.5.

## References

EDI \(Environmental Data Initiative\). 2019. Five phases of data publishing - Phase 2: Format and QC data tables. [https://environmentaldatainitiative.org/five-phases-of-data-publishing/phase-2/](https://environmentaldatainitiative.org/five-phases-of-data-publishing/phase-2/)

EML \(Ecological Metadata Language\). 2019. Ecological Metadata Language Version 2.2.0. [https://doi.org/10.5063/F11834T2](https://doi.org/10.5063/F11834T2)

Evans, K., et al. 2016. ESDS-RFC-027v1.1 - ASCII File Format Guidelines for Earth Science Data. [https://cdn.earthdata.nasa.gov/conduit/upload/4827/ESDS-RFC-027v1.1.pdf](https://cdn.earthdata.nasa.gov/conduit/upload/4827/ESDS-RFC-027v1.1.pdf)

FGDC \(Federal Geographic Data Committee\). 2016. National Geospatial Data Assets \(NGDA\) Metadata Guidelines, Version 3. [https://www.geoplatform.gov/wpcontent/](https://www.geoplatform.gov/wpcontent/) uploads/2018/05/NGDA\_Metadata\_Guidelines\_v3.pdf

Pepler, S., Parton, G. \(2009\) The BADC Text File Guide for users, and producers. Documentation. [https://help.ceda.ac.uk/article/105-badc-csv](https://help.ceda.ac.uk/article/105-badc-csv)

Shafranovich, Y. \(2005\) RFC 4180 - Common Format and MIME Type for Comma-Separated Values \(CSV\) Files. [https://tools.ietf.org/html/rfc4180](https://tools.ietf.org/html/rfc4180)

 
