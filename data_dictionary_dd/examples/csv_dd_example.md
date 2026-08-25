# CSV Data Dictionary example template

| column_or_row_name | unit | definition | column_or_row_long_name | data_type |
| :--- | :--- | :--- | :--- | :--- |
| area | N/A | Name of the intensive field site within the project. Possible values: Area A, Area B, Area C | Field site name | text |
| date\_collected | yyyy-mm-dd | Date samples were collected in the field. | N/A | date |
| sample\_ID | N/A | Samples were collected in the field and bags marked with sequential ID numbers. | Unique sample identifier | text |
| long | decimal degrees | Longitude provided in WGS84 | Longitude | numeric |
| lat | decimal degrees | Latitude provided in WGS84 | Latitude | numeric |
| sample\_volume\_collected | mg/L | The volume of the sample collected. | The volume of the sample collected. | numeric |
| sample\_type | N/A | Type of sample collection method.   Possible values: ISCO, surface\_grab | N/A | N/A |
| Fl | mg/L | Fluoride concentration.  Missing data = -9999 | Fluoride | numeric |
| Cl | mg/L | Chloride concentration | Chloride | numeric |
| Ca | mg/L | Calcium concentration | Calcium | numeric |

