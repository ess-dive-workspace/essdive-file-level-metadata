# ESS-DIVE File Level Metadata Reporting Format v1.1.2

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
## Updates in v1.1.2
The File Level Metadata reporting format was updated in August of 2025 to address feedback from adopters. The changes made in v1.1.2 focused on providing clarification on metadata fields within the file level metadata and data dictionary files, and providing examples for the use of header_rows and column_or_row_name_position fields. No changes were made to the templates directly.

* Provide clarity for header_rows field definition (File Level Metadata)
    * Revise the definition of the header_rows field to provide additional clarity to avoid misinterpretation
    * Revise the definition of the header_rows field to provide links to the example images
* Revise column_or_row_name_position field description to include examples (File Level Metadata)
    * Revise the definition of the column_or_row_name_position field to provide links to the example images
* Incorporate examples of using header_rows and column_or_row_name_position fields (File Level Metadata)
    * Provide examples of using the header_rows and column_or_row_name_position fields: [example 1](flmd_header_rows_example_1.png), [example 2](flmd_header_rows_example_2.png), [example 3](flmd_header_rows_example_3.png)
* Revise FLMD instructions file (File Level Metadata)
    * Provide clarity on the use of the header_rows and column_or_row_name_position fields and link to examples within the FLMD instructions
* Provide clarity for missing_value_code field (Data Dictionary)
    * Provide clarity on the missing_value_code, including that the field is to be used to specify a single missing value code

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

 
