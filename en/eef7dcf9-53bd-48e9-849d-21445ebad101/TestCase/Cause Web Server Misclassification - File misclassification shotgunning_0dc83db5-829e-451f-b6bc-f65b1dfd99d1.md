{
  "id": "85",
  "name": "Cause Web Server Misclassification - File misclassification shotgunning",
  "description": "An attacker makes changes to file extensions and MIME types typically processed by web servers and looks for abnormal behavior.\n\nAttack Step Techniques:\n1.   Attacker submits files with switched extensions (e.g. .php on a .jsp file) to web server.\nenv-Web\n\n2.   Attacker adds extra characters (e.g. adding an extra . after the file extension) to filenames of files submitted to web server.\nenv-Web\n\nIndicators: \n1.  Positive,  The web server uses the wrong handler to execute the file, as expected by the attacker.\nenv-Web\n\n2\tInconclusive,  No result from the web server.\nenv-Web\n\n3.   Negative,  The web server ignore the manipulation and process the request has it should have been.\nenv-Web\n\nOutcomes\n1.  Success,  Web server exhibits unexpected behavior.\n\n2.   Failure,   The attacker cannot get the web server to misclassify a file.\n\nSecurity Controls:\n1.   Detective,  Monitor web server logs for excessive file processing errors\n\n2.   Preventative,  Always validate that file content structure matches implicitly or explicitly declared file type as first step of processing.\n\nReference: https://capec.mitre.org/data/definitions/11.html\n",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "0dc83db5-829e-451f-b6bc-f65b1dfd99d1",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}