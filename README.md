# ESS-DIVE File Level Metadata Reporting Format v2.0.0
_**Attention:** Previous versions (v1) of this reporting format are being phased out. We strongly recommend that you migrate to the latest version of the reporting format (v2.0.0)._

## About the reporting format
File level metadata provides granular information at the file level to enable comparison of files within a data set and the ability to search for and locate files across the data collection.

## Quickstart guide

The FLMD and data dictionary reporting formats are organized into separate folders as they can be used separately or together. For each of the reporting formats:
1. **Read** the instruction documents to understand how to fill out the templates.
2. **Review** the terminology guides and controlled vocabularies to understand definitions and requirements of each term used in the templates.
3. **Download** a blank copy of the reporting format templates.
4. **Save** your completed reporting format templates as CSV files and upload them to ESS-DIVE as part of your dataset.

---  
## Updates in v2.0.0
The File Level Metadata reporting format was updated in November 2026 to improve consistency between the File Level Metadata and Data Dictionary components and to address feedback from adopters. The changes in v2.0.0 include:
- Reorganized the repository into two parallel folders — `file_level_metadata_flmd/` and `data_dictionary_dd/` — so each component has its own template, instructions, term guide, controlled vocabulary, and examples.
- Added a new `data_dictionary_file_name` term to the FLMD template to formally link data files to their associated data dictionary.
- Replaced quick guides with structured term guides that document each term’s requirement level, format, definition, example, and additional guidance.
- Added standalone controlled vocabulary documents for both the FLMD (`standard`, `data_orientation`) and DD (`data_type`, `unit`).
- Expanded DD instructions to describe a third linking option (1:Multiple DDs).

File Level Metadata versions 2.x.x are not backwards compatible with prior versions 1.x.x. Version 1.1.2 will be retired on April 1, 2027.

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

## References

EDI \(Environmental Data Initiative\). 2019. Five phases of data publishing - Phase 2: Format and QC data tables. [https://environmentaldatainitiative.org/five-phases-of-data-publishing/phase-2/](https://environmentaldatainitiative.org/five-phases-of-data-publishing/phase-2/)

EML \(Ecological Metadata Language\). 2019. Ecological Metadata Language Version 2.2.0. [https://doi.org/10.5063/F11834T2](https://doi.org/10.5063/F11834T2)

Evans, K., et al. 2016. ESDS-RFC-027v1.1 - ASCII File Format Guidelines for Earth Science Data. [https://cdn.earthdata.nasa.gov/conduit/upload/4827/ESDS-RFC-027v1.1.pdf](https://cdn.earthdata.nasa.gov/conduit/upload/4827/ESDS-RFC-027v1.1.pdf)

FGDC \(Federal Geographic Data Committee\). 2016. National Geospatial Data Assets \(NGDA\) Metadata Guidelines, Version 3. [https://www.geoplatform.gov/wpcontent/](https://www.geoplatform.gov/wpcontent/) uploads/2018/05/NGDA\_Metadata\_Guidelines\_v3.pdf

Pepler, S., Parton, G. \(2009\) The BADC Text File Guide for users, and producers. Documentation. [https://help.ceda.ac.uk/article/105-badc-csv](https://help.ceda.ac.uk/article/105-badc-csv)

Shafranovich, Y. \(2005\) RFC 4180 - Common Format and MIME Type for Comma-Separated Values \(CSV\) Files. [https://tools.ietf.org/html/rfc4180](https://tools.ietf.org/html/rfc4180)

 
