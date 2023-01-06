{
  "id": "9",
  "name": "Authorization Bypass - Path Traversal Input Vectors Enumeration",
  "description": "<p></p><p>In order to determine which part of the application is vulnerable to input validation bypassing, the tester needs to enumerate all parts of the application which accept content from the user. This also includes HTTP GET and POST queries and common options like file uploads and HTML forms.\n\nHere are some examples of the checks to be performed at this stage:\n\n    Are there request parameters which could be used for file-related operations?\n    Are there unusual file extensions?\n    Are there interesting variable names? \n\nhttp://example.com/getUserProfile.jsp?item=ikki.html\nhttp://example.com/index.php?file=content\nhttp://example.com/main.cgi?home=index.htm\n\nIs it possible to identify cookies used by the web application for the dynamic generation of pages/templates? \n\nCookie: ID=d9ccd3f4f9f18cc1:TM=2166255468:LM=1162655568:S=3cFpqbJgMSSPKVMV:TEMPLATE=flower\nCookie: USER=1826cc8f:PSTYLE=GreenDotRed\n\ntest</p>",
  "labels": "",
  "libraryId": "1",
  "guid": "528ed098-d309-42f9-a90e-570bc3e6c74f",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}