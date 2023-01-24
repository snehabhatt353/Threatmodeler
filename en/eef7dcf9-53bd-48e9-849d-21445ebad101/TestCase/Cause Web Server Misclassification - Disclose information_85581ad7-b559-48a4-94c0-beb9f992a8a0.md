{
  "id": "87",
  "name": "Cause Web Server Misclassification - Disclose information",
  "description": "The attacker, by manipulating a file extension or MIME type is able to make the web server return raw information (not executed).\n\nAttack Step Techniques: \n1.  Manipulate the file names that are explicitly sent to the server.\nenv-Web\n\n2.  Manipulate the MIME sent in order to confuse the web server.\nenv-Web\n\nOutcomes\n1.  Success,  The attacker gets the information from the server\n\nSecurity Controls\n1.  Preventative,  Always validate that file content structure matches implicitly or explicitly declared file type as first step of processing.\n\nReference: https://capec.mitre.org/data/definitions/11.html ",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "85581ad7-b559-48a4-94c0-beb9f992a8a0",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}