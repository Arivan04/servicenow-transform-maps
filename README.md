# Import Data Using Transform Maps

A small ServiceNow project that imports employee data from an Excel spreadsheet into a custom Employee table using Import Sets and Transform Maps.

## What this project does

The spreadsheet is uploaded to ServiceNow as a data source and loaded into an import set table. A Transform Map is then used to map the spreadsheet fields to the Employee table.

Employee ID is used as the coalesce field. This lets ServiceNow update an existing employee when the same ID is imported again instead of creating a duplicate record.

After the import, the employee data is used to create reports and an Employee Analytics dashboard.

## Workflow

1. Prepare the employee data in an Excel spreadsheet.
2. Upload the spreadsheet as a ServiceNow Data Source.
3. Load the data into an Import Set.
4. Create a Transform Map between the import table and Employee table.
5. Configure the required field mappings.
6. Set Employee ID as the coalesce field.
7. Run the transformation and verify the imported records.
8. Create reports from the employee data.
9. Add the reports to the Employee Analytics dashboard.

## ServiceNow features used

- Data Sources
- Import Sets
- Transform Maps
- Field Maps
- Coalesce
- Custom tables
- Reports
- Dashboards

## Sample data

The spreadsheet used for this project contains test data only. The employee names and other records are fictional and are included only to demonstrate the import process.

The spreadsheet is available in the `data/` directory.

## Demo

A screen recording of the complete project workflow is provided separately with the project submission.

## Notes

This repository mainly contains the project documentation and input spreadsheet. Most of the implementation is configuration performed inside ServiceNow rather than conventional source code.
