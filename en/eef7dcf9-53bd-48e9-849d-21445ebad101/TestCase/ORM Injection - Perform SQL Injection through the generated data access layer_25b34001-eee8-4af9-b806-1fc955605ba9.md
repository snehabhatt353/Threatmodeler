{
  "id": "63",
  "name": "ORM Injection - Perform SQL Injection through the generated data access layer",
  "description": "An attacker proceeds to exploit a weakness in the generated data access methods that does not properly separate control plane from the data plan, or potentially a particular way in which developer might have misused the generated code, to modify the structure of the executed SQL queries and/or inject entirely new SQL queries.\n\nAttack Step Techniques:\nAn attacker uses normal SQL injection techniques and adjusts them to reflect the type of data access layer generation framework used by the application.\nenv-Web\n\nOutcomes\n1.\tSuccess\t\nAttacker achieves goal of unauthorized system access, denial of service, etc.\n\n2.\tFailure\t\nAttacker unable to exploit SQL Injection vulnerability.\n\n\nReference: https://capec.mitre.org/data/definitions/109.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "25b34001-eee8-4af9-b806-1fc955605ba9",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}