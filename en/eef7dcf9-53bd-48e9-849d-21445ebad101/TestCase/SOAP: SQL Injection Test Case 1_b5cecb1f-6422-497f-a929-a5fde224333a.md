{
  "id": "33",
  "name": "SOAP: SQL Injection Test Case 1",
  "description": "SQL Injection the art of sending in SQL Statements in forms and data to the target system to be executed by the back end database. The result we're looking for is will either for the system to allow you access or to display information that will move us closer to getting access. In the infancy of The Web, this used to be a large problem, but is largely handled today at least on a basic level. Unfortunately with in the realm of SOA development we've taken a step back and the database is exposed surprisingly often.\n\nWhat we'll be looking at here is using several small steps to see if the base security is fine in regards to Data Injection.\n\nStep 1: Random SQL\nWe'll start of with a simple test, we insert a SQL Statement in any field and monitor the return response.\n\n<login>\n  <username><User>SELECT * from userstable</username>\n  <password>*</password>\n</login>\n\nThis might seem way to simple, but look at this message:\n\nMicrosoft OLE DB Provider for ODBC Drivers error '80040e07' [Microsoft]\n[ODBC SQL Server Driver][SQL Server]Syntax error Invalid string or buffer length.\n\nWe have already gained information about what what the database is, we can probably guess what the platform used to create the Web Services are and can use that information in further attacks.\n\n\n[Source] soapui.org",
  "labels": "",
  "libraryId": "1",
  "guid": "b5cecb1f-6422-497f-a929-a5fde224333a",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}