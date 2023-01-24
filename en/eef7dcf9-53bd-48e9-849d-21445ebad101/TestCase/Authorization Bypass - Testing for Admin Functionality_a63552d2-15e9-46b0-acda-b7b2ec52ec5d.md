{
  "id": "11",
  "name": "Authorization Bypass - Testing for Admin Functionality",
  "description": "For example, suppose that the 'AddUser.jsp' function is part of the administrative menu of the application, and it is possible to access it by requesting the following URL:\n\n    https://www.example.com/admin/addUser.jsp \n\nThen, the following HTTP request is generated when calling the AddUser function: \n\nPOST /admin/addUser.jsp HTTP/1.1\nHost: www.example.com\n[other HTTP headers]\n\nuserID=fakeuser&role=3&group=grp001\n\nWhat happens if a non-administrative user tries to execute that request? Will the user be created? If so, can the new user use her privileges?\n\nTesting for access to resources assigned to a different role\nAnalyze, for example, an application that uses a shared directory to store temporary PDF files for different users. Suppose that documentABC.pdf should be accessible only by the user test1 with roleA. Verify if user test2 with roleB can access that resource.\n\nResult Expected:\nTry to execute administrative functions or access administrative resources as a standard user.",
  "labels": "",
  "libraryId": "1",
  "guid": "a63552d2-15e9-46b0-acda-b7b2ec52ec5d",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}