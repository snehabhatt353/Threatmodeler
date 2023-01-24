{
  "id": "37",
  "name": "SOAP: SQL Injection Test Case 5 - Type Conversions",
  "description": "We can also try exposing the database by trying sending in type conversions that surely will fail in the database.\n\n<login>\n  <username>CAST('eviware' AS SIGNED INTEGER)</username>\n  <password>yesitdoes!</password>\n</login>\n\nThe goal here is -as with the above- to make the database give us any info by sending an error message that exposes the database. As we said earlier, anything that exposes what the database or the application platform is using is helpful, it can help us look up specific vulnerabilities for that environment.",
  "labels": "",
  "libraryId": "1",
  "guid": "03de368c-cae9-4a7d-9581-e1b8943d2fd3",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}