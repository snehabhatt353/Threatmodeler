{
  "id": "84",
  "name": "Cause Web Server Misclassification - Footprint file input vectors",
  "description": "Manually or using an automated tool, an attacker searches for all input locations where a user has control over the filenames or MIME types of files submitted to the web server.\n\nAttack Step Techniques:\n1.  Attacker manually crawls application to identify file inputs\nenv-Web\n\n2.  Attacker uses an automated tool to crawl application identify file inputs\nenv-Web\n\n3.  Attacker manually assesses strength of access control protecting native application files from user control\nenv-Web\n\n4.  Attacker explores potential for submitting files directly to the web server via independently constructed HTTP Requests\nenv-Web\n\nIndicators\n1.  Positive,  Application submits files under user control to the web server\nenv-Web\n\n2.  Negative,  Application does not submit files under user control to the web server\nenv-Web\n\n3.   Negative,  Application strictly protects all native application files from user control\nenv-Web\n\nOutcomes:\n1.  Success,  User-controllable files are identified\n\nReference: https://capec.mitre.org/data/definitions/11.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "2e6f86ba-64b0-42ca-911c-ef78813bf150",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}