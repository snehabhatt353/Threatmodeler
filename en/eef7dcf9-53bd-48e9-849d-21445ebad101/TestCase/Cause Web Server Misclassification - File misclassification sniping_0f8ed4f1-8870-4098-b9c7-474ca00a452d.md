{
  "id": "86",
  "name": "Cause Web Server Misclassification - File misclassification sniping",
  "description": "Understanding how certain file types are processed by web servers, an attacker crafts varying file payloads and modifies their file extension or MIME type to be that of the targeted type to see if the web server is vulnerable to misclassification of that type.\n\nAttack Step Techniques:\n1.  Craft a malicious file payload, modify file extension to the targeted file type and submit it to the web server.\nenv-Web\n\n2.  Craft a malicious file payload, modify its associated MIME type to the targeted file type and submit it to the web server.\nenv-Web\n\nIndicators:\n1.  Positive,  The web server uses the wrong handler to execute the file, as expected by the attacker.\nenv-Web\n\n2.  Inconclusive,  No result from the web server.\nenv-Web\n\n3.  Negative, The web server ignore the manipulation and process the request has it should have been.\nenv-Web\n\nOutcomes:\n1.  Success,  Attacker's payload is acted on by web server.\n2.   Failure,  The attacker cannot get the web server to misclassify a file.\n\nSecurity Controls:\n1.  Detective,  Monitor web server logs for excessive file processing errors\n2.  Preventative,  Always validate that file content structure matches implicitly or explicitly declared file type as first step of processing.\n\nReference: https://capec.mitre.org/data/definitions/11.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "0f8ed4f1-8870-4098-b9c7-474ca00a452d",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}