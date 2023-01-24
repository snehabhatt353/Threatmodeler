{
  "id": "110",
  "name": "Dictionary based Password Attack - Determine applications and or systems password policy",
  "description": "Determine the password policies of the target application/system.\n\nAttack Step Techniques:\n1.    Determine minimum and maximum allowed password lengths.\nenv-All\n\n2.   Determine format of allowed passwords (whether they are required or allowed to contain numbers, special characters, etc., or whether they are allowed to contain words from the dictionary).\nenv-All\n\n3.   Determine account lockout policy (a strict account lockout policy will prevent brute force attacks).\nenv-All\n\nIndicators:\n1.   Positive,    Passwords are used in the application/system\nenv-All\n2.   Negative,   Passwords are not used in the application/system.\nenv-All\n\nReference: https://capec.mitre.org/data/definitions/16.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "6cd4e9fa-6a58-4937-9a13-ba1d81be4aa5",
  "isHidden": true,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}