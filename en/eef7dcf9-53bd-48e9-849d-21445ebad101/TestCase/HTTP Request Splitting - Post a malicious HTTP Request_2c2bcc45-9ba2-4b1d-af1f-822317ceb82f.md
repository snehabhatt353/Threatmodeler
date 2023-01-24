{
  "id": "74",
  "name": "HTTP Request Splitting - Post a malicious HTTP Request",
  "description": "Post a malicious HTTP request that will be interpreted as multiple HTTP requests when parsed on the server\n\nAttack Step Techniques: \n1.  Post a malicious HTTP Request utilizing double CR/LF characters in HTTP header to cause request splitting\nenv-Web\n\n2.   Post a malicious HTTP Request utilizing \"Transfer Encoding: chunked\" in the request header to cause request splitting\nenv-Web\n\n3.   Post a malicious HTTP Request utilizing double Content-Length headers to cause request splitting\nenv-Web",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "2c2bcc45-9ba2-4b1d-af1f-822317ceb82f",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}