{
  "id": "61",
  "name": "ORM Injection - Determine Persistence Framework Used",
  "description": "An attacker tries to determine what persistence framework is used by the application in order to leverage a weakness in the generated data access layer code or a weakness in a way that the data access layer may have been used by the developer.\n\nAttack Step Techniques:\nAn attacker provides input to the application in an attempt to induce an error screen that reveals a stack trace that gives an indication of the automated data access layer used. Or an attacker may simply make some educated guesses and assume, for instance, that Hibernate is used and try to craft an attack from there.\n\nReference: https://capec.mitre.org/data/definitions/109.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "070f5226-aa7d-4cec-a532-9c632a0e8124",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}