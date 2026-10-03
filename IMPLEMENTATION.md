# Implementation Notes

## Data import

The employee spreadsheet was added to ServiceNow as a file-based Data Source. ServiceNow loaded the spreadsheet rows into an Import Set table before transformation.

## Transform Map

A Transform Map was created to move data from the imported spreadsheet fields into the Employee table. The spreadsheet columns were mapped to their corresponding fields in the target table.

## Coalesce

Employee ID was configured as the coalesce field.

When ServiceNow processes a row, it checks whether an Employee record with the same Employee ID already exists:

- If a matching record exists, that record is updated.
- If no matching record exists, a new record is inserted.

This avoids creating duplicate employee records when updated spreadsheet data is imported.

## Verification

After running the transformation, the Employee table was checked to confirm that the spreadsheet records had been imported correctly.

Reports were then created from the imported employee data and added to an Employee Analytics dashboard.

## Demo

The submitted demo video shows the spreadsheet, import configuration, Transform Map and field mappings, transformation results, reports, and final dashboard.
