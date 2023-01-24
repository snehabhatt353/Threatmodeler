{
  "id": "71",
  "name": "Session Management Test Case",
  "description": "All interaction between the client and application should be tested at least against the following criteria:\n\n    Are all Set-Cookie directives tagged as Secure?\n    Do any Cookie operations take place over unencrypted transport?\n    Can the Cookie be forced over unencrypted transport?\n    If so, how does the application maintain security?\n    Are any Cookies persistent?\n    What Expires= times are used on persistent cookies, and are they reasonable?\n    Are cookies that are expected to be transient configured as such?\n    What HTTP/1.1 Cache-Control settings are used to protect Cookies?\n    What HTTP/1.0 Cache-Control settings are used to protect Cookies? \n\nReference: https://www.owasp.org/index.php/Testing_for_Exposed_Session_Variables_(OTG-SESS-004)",
  "labels": "",
  "libraryId": "1",
  "guid": "b7793d50-cf8e-449b-bd92-5abbbf51a98a",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}