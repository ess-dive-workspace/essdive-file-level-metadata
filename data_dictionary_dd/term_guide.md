# Term Guide
The data dictionary terms are defined below, including whether that term is required, a brief definition, formatting requirements, an example, and additional guidance. 

### Terms of the reporting format:
* [column_or_row_name](#column_or_row_name)  
* [unit](#unit)  
* [definition](#definition)
* [column_or_row_long_name](#column_or_row_long_name)
* [data_type](#data_type)
* [missing_value_code](#missing_value_code)

---  
### column_or_row_name
|term|`column_or_row_name`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|required|
|format|free text|
|definition|Column or row header name from the data file. Provide entries for each column or row name from the matrix in the data file.|
|example|temp_soil_2|
|additional guidance|Column or row header name can be any text. Information will not be parsed from the header name.|

### unit
|term|`unit`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|required|
|format|free text|
|definition|Unit of measurement.|
|example|degree Celsius|
|additional guidance|Insert "N/A" when units aren't applicable. <br><br>Strongly recommended to follow the [Unified Code of Unified Measurements (UCUM)](https://ucum.org/ucum) controlled vocabulary for units. <br><br>For date and datetime data types, you may use this term to indicate the format (e.g., YYYY-MM-DD hh:mm:ss).|

### definition
|term|`definition`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|required|
|format|free text|
|definition|A description of the column/row header.|
|example|Soil temperature replicate 2 at location loc_25d|
|additional guidance|N/A|

### column_or_row_long_name
|term|`column_or_row_long_name`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|recommended|
|format|free text|
|definition|Longer human-readable column or row name. Sometimes this may be identical to `definition` or `column_or_row_name`.|
|example|temperature soil 2|
|additional guidance|N/A|

### data_type
|term|`data_type`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|optional|
|format|[Controlled vocabulary](https://github.com/ess-dive-workspace/essdive-file-level-metadata/blob/release-v1.2.0/data_dictionary_dd/controlled_vocabulary.md#data_type)|
|definition|A description of the column/row header.|
|example|Soil temperature replicate 2 at location loc_25d|
|additional guidance|N/A|

### missing_value_code
|term|`missing_value_code`|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement|optional|
|format|free text|
|definition|The missing value code used for missing measurements. Only one code allowed.|
|example|-9999|
|additional guidance|Based on the CSV Reporting Format guidelines, for columns containing numeric data, ESS-DIVE recommends using "-9999" as the missing value code. For columns containing character data, ESS-DIVE recommends using "N/A" as the missing value code. If you would like to use a different missing value code, specify the used missing value code within this term. <br><br>If a missing value code is not applicable for a column, leave this entry blank or use a generic missing value code.|
