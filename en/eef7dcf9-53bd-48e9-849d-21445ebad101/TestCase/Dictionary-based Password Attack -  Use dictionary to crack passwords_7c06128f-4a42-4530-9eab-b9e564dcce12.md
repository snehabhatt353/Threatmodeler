{
  "id": "113",
  "name": "Dictionary-based Password Attack -  Use dictionary to crack passwords",
  "description": "Use a password cracking tool that will leverage the dictionary to feed passwords to the system and see if they work.\n\nAttack Step Techniques:\n1.   Try all words in the dictionary, as well as common misspellings of the words as passwords for the chosen username(s).\nenv-All\n\n2.   Try common combinations of words in the dictionary, as well as common misspellings of the combinations as passwords for the chosen username(s).\nenv-All\n\nIndicators:\n1\tNegative,   Application/system does not use password authentication.\nenv-All\n\nOutcomes:\n1\tSuccess,   Attacker determines correct password for a user ID and obtains access to application or system.\n2\tFailure,    Attacker is unable to determine correct password for a user ID and obtain access to application or system.\n\nSecurity Controls:\n1\tDetective,    Large number of authentication failures in logs.\n2\tPreventative,    Enforce strict account lockout policies.\n3\tPreventative,    Enforce strong passwords (having sufficient length and containing mix of lower case and upper case letters, numbers, and special characters)\n\nreference: https://capec.mitre.org/data/definitions/16.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "7c06128f-4a42-4530-9eab-b9e564dcce12",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}