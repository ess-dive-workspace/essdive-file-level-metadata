# CSV Data Dictionary quick guide

Elements of the data dictionary:

* [column_or_row_name](#column-or-row-name)  
* [unit](#unit)  
* [definition](#definition)  
* [column_or_row_long_name](#column-or-row-long-name)  
* [data_type](#data-type)
* [missing_value_code](#missing-value-code)

## Column or Row Name

| Metadata\_Element | column_or_row_name |
| :--- | :--- |
| Reporting format statement | Column or row name from the data file. |
| Reporting format definition | Provide entries for each column or row name from the data matrix in the data file. |
| Required, Recommended or Optional | required |

## Unit

| Metadata\_Element | unit |
| :--- | :--- |
| Reporting format statement | Provide the format or variable unit of measurement. |
| Reporting format definition | Provide variable units of measurement. Insert "N/A" when units aren't applicable. Data should be represented with units of measurement approved by the International System of Units \(SI\). Non-SI units are accepted for use and should be defined and referenced. |
| Required, Recommended or Optional | required |

## Definition

| Metadata\_Element | definition |
| :--- | :--- |
| Reporting format statement | A complete unambiguous description. |
| Reporting format definition | A complete unambiguous description. Information may include: formulas used to calculate entry; definitions of coding systems \(e.g. missing values, quality flags, etc.\); detection limits; timestamp calculation; measurement of uncertainty, etc. |
| Required, Recommended or Optional | required |

## Column or Row Long Name

| Metadata\_Element | column_or_row_long_name |
| :--- | :--- |
| Reporting format statement | Human-readable name. |
| Reporting format definition | Longer human-readable column or row name. Sometimes this may be identical to Definition or even Column\_or\_Row\_Name. |
| Required, Recommended or Optional | recommended |

## Data type

| Metadata\_Element | data_type |
| :--- | :--- |
| Reporting format statement | Define the data type. |
| Reporting format definition | Define the data type for each column \(e.g. text, numeric, date\) |
| Required, Recommended or Optional | recommended |

### Missing Value Code

| Metadata\_Element |missing_value_code|
| :--- | :--- |
|Reporting format statement| Report missing value code. |
|Reporting format definition|Report a single missing value code for each column, if applicable. Based on the [CSV reporting format guidelines](https://ess-dive.gitbook.io/csv-file-structure-reporting-format), for columns containing numeric data, we recommend you use "-9999" as the missing value code. For columns containing character data, we recommend you use "N/A" as the missing value code. If you would like to use a different missing value code, specify the used missing value code within this field. If a missing value code is not applicable for a column, leave this entry blank.|
|Required, Recommended or Optional|optional|


