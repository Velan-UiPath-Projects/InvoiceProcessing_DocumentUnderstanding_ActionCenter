Invoice Extraction Project

Objective:
The objective of this project is to automate the extraction of specific information from Super Stores invoices. The extracted information includes Invoice Number, Customer Name, Invoice Date, Order ID, Total, and Balance. Once the information is extracted, it will be sent to an Admin for validation. Upon approval, the extracted data must be updated to an SQL table.

Process Overview:

Invoice Processing Workflow:

Input: Super Stores Invoices (PDF or image format)

Output: Extracted information (Invoice Number, Customer Name, Invoice Date, Order ID, Total, Balance)

Steps:
Load the invoice document using UiPath.IntelligentOCR.Activities.
Use UiPath.DocumentUnderstanding.ML.Activities for data extraction.
Validate the extracted data.
If data validation is successful, update the SQL table using UiPath.Database.Activities.

Activities Used:

UiPath.DocumentUnderstanding.ML.Activities (Version: 1.21.3)
UiPath.IntelligentOCR.Activities (Version: 6.9.6)
UiPath.Persistance.Activities (Version: 1.5.5)
UiPath.FormActivityLibrary.Contracts (Version: 2.0.7)
UiPath.Database.Activities (Version: 1.7.1)


Process Steps:

Initialization:
Initialize variables and set up environment configurations.

Load Invoice Document:
Use UiPath.IntelligentOCR.Activities to load Super Stores invoices in PDF or image format.

Extract Information:
Utilize UiPath.DocumentUnderstanding.ML.Activities to extract the following information:
Invoice Number
Customer Name
Invoice Date
Order ID
Total
Balance
Validate Extracted Data:

Implement validation checks to ensure the accuracy and completeness of extracted information.

If any discrepancies are found, handle them appropriately.

Send Data for Admin Validation:

Send the extracted data to the Admin for manual validation.

Wait for approval or feedback.

Update SQL Table:
If the Admin approves the extracted data:
Utilize UiPath.Database.Activities to update the SQL table with the extracted information.
If not approved, handle the rejection and log the feedback for further analysis.


Completion and Error Handling:
Log completion status and any errors encountered during the process.
Implement error handling mechanisms to handle exceptions gracefully.

Conclusion:
The Invoice Extraction Project automates the extraction of key information from Super Stores invoices and updates an SQL table with the validated data. By leveraging UiPath activities, the process enhances efficiency and reduces manual effort in invoice processing tasks.






