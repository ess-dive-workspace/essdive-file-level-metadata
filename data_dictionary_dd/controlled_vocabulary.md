# Controlled Vocabulary
The File Level Metadata controlled vocabularies for applicable terms in the data dictionary file template can be found below.

### Controlled vocabularies are available for the following terms:
- [unit](#unit)
- [data_type](#data_type)

---
## unit
The controlled vocabulary for the unit is based on the [Quantities, Units, Dimensions, and Types (QUDT)](https://www.qudt.org/doc/DOC_VOCAB-UNITS.html). The Definition provided for the controlled vocabulary is based upon the QUDT term name. For units not listed below, please visit QUDT to select the standardized unit vocabulary. Only if you cannot find your unit in QUDT, enter a custom unit.
|Controlled Vocabulary|Definition|
|:----------------------------------------------------|:----------------------------------------------------|
|UNITLESS|Unitless. http://qudt.org/vocab/unit/UNITLESS|
|DEG_C|Degree Celsius. https://qudt.org/vocab/unit/DEG_C|
|MicroS-PER-CentiM|Microsiemens per Centimetre (Centimeter). http://qudt.org/vocab/unit/MicroS-PER-CentiM|
|MilliGM-PER-L|Milligram per Litre (Liter). http://qudt.org/vocab/unit/MilliGM-PER-L|
|PH|Acidity (pH). http://qudt.org/vocab/unit/PH|
|MOL-PER-KiloGM|Mole per Kilogram. http://qudt.org/vocab/unit/MOL-PER-KiloGM|
|MOL-PER-L|Mole per Litre (Liter). http://qudt.org/vocab/unit/MOL-PER-L|
|PERCENT|Percent. http://qudt.org/vocab/unit/PERCENT|
|PERMILLE|Permille (Per Mille). http://qudt.org/vocab/unit/PERMILLE|
|COUNT|Count. http://qudt.org/vocab/unit/COUNT|
|MilliL|Millilitre (Milliliter). http://qudt.org/vocab/unit/MilliL|
|L|Litre (Liter). http://qudt.org/vocab/unit/L|
|MilliM|Millimetre (Millimeter). http://qudt.org/vocab/unit/MilliM|
|CentiM|Centimetre (Centimeter). http://qudt.org/vocab/unit/CentiM|
|M|Metre (Meter). http://qudt.org/vocab/unit/M|
|KiloM|Kilometre (Kilometer). http://qudt.org/vocab/unit/KiloM|
|MilliGM|Milligram. http://qudt.org/vocab/unit/MilliGM|
|GM|Gram. http://qudt.org/vocab/unit/GM|
|KiloGM|Kilogram. http://qudt.org/vocab/unit/KiloGM|
|FT|Foot (Feet). http://qudt.org/vocab/unit/FT|

## data_type
|Controlled Vocabulary| Definition |
|:----------------------------------------------------|:----------------------------------------------------|
| text | Alphanumeric values. Numbers will be treated as text / strings. Includes: str, character. |
| numeric | A number. Includes: float, decimal |
| date | A calendar date without a time. |
| datetime | A calendar date and time. |
| enum | A set of predefined options or codes. The enums may be provided by the data contributor or developed by ESS-DIVE as part of a reporting format. |
| integer | A whole number with no decimal or fractional value. |
