{
  "id": "35",
  "name": "SOAP: SQL Injection Test Case 3 - Classic Single Quote",
  "description": "This test is the most common SQl injection test using the following:\n\n          \n<login>\n  <username> ' or 1=1--</username>\n  <password>' or 1=1--</password>\n</login>\n\n\"Why?\", you might ask. Well, if the SQL used to check the login is:\n\nSELECT * FROM users WHERE username = '[username]' AND password ='[password]';\n\nThis results in the following if the contents of the elements aren't checked:\n\nSELECT * FROM users WHERE username = '' or 1=1 - -' AND password ='[password]';\n\nWhich might actually cause the SQL Server to exclude everything after ?--\" (since it's TransactionSQL) and just return the first user in the database. With some (bad)luck, we might even be able to log in.",
  "labels": "",
  "libraryId": "1",
  "guid": "d479e5db-3286-4824-a3d3-a65b7dabd06d",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}