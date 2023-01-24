{
  "id": "125",
  "name": "Authentication Bypass- Direct page request",
  "description": "If a web application implements access control only on the log in page, the authentication schema could be bypassed.\n For example, if a user directly requests a different page via forced browsing, that page may not check the credentials of the user before granting access. Attempt to directly access a protected page through the address bar in your browser to test using this method. \n\nReference: https://www.owasp.org/index.php/Testing_for_Bypassing_Authentication_Schema_(OTG-AUTHN-004)\n\n",
  "labels": "OWASP",
  "libraryId": "1",
  "guid": "062b0a28-4d9f-4bcb-bed7-0bb5b79ada64",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}