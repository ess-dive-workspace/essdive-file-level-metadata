# Controlled Vocabulary
The File Level Metadata controlled vocabularies for applicable terms in the data dictionary file template can be found below.

### Controlled vocabularies are available for the following terms:
- [unit](#unit)
- [data_type](#data_type)

---
## unit
The controlled vocabulary for the unit is based on the [Unified Code of Unified Measurements (UCUM)](https://ucum.org/ucum). The Definition provided for the controlled vocabulary is the UCUM code.
|Controlled Vocabulary|Definition|
|:----------------------------------------------------|:----------------------------------------------------|
|unitless|unitless|
|degree Celsius|Cel|
|microsiemens per centimeter|uS/cm|
|milligram per liter|mg/L|
|percent saturation|%{saturation}|
|pH|[pH]|
|moles per kilogram|mol/kg|
|moles per liter|mol/L|
|percent|%|
|per mille|/10*2|
|count|{count}|
|milliliter|mL|
|liter|L|
|millimeter|mm|
|centimeter|cm|
|meter|m|
|kilometer|km|
|milligram|mg|
|gram|g|
|kilogram|kg|
|feet (international)|[ft_i]|

## data_type
|Controlled Vocabulary| Definition |
|:----------------------------------------------------|:----------------------------------------------------|
| text | Includes: str, character. Numbers will be treated as text / strings. |
| numeric | Includes: float, decimal |
| date | A calendar date without a time. |
| datetime | A calendar date and time. |
| enum | A set of predefined options or codes. |
| integer | A whole number with no decimal or fractional value. |
