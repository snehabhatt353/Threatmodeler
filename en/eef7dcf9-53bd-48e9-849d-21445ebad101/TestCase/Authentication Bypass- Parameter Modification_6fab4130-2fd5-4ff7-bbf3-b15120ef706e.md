{
  "id": "126",
  "name": "Authentication Bypass- Parameter Modification",
  "description": "Another problem related to authentication design is when the application verifies a successful log in on the basis of a fixed value parameters. A user could modify these parameters to gain access to the protected areas without providing valid credentials.\n\n In the example below, the \"authenticated\" parameter is changed to a value of \"yes\", which allows the user to gain access. In this example, the parameter is in the URL, but a proxy could also be used to modify the parameter, especially when the parameters are sent as form elements in a POST request or when the parameters are stored in a cookie.\n\nhttp://www.site.com/page.asp?authenticated=no \nraven@blackbox /home $nc www.site.com 80                    \nGET /page.asp?authenticated=yes HTTP/1.0                    \n                                                            \nHTTP/1.1 200 OK                                             \nDate: Sat, 11 Nov 2006 10:22:44 GMT                         \nServer: Apache                                              \nConnection: close                                           \nContent-Type: text/html; charset=iso-8859-1                 \n \n<!DOCTYPE HTML PUBLIC \"-//IETF//DTD HTML 2.0//EN\">          \n<HTML><HEAD>                                                \n</HEAD><BODY>                                               \n<H1>You Are Authenticated</H1>                              \n</BODY></HTML>\n\nReference: https://www.owasp.org/index.php/Testing_for_Bypassing_Authentication_Schema_(OTG-AUTHN-004) ",
  "labels": "OWASP",
  "libraryId": "1",
  "guid": "6fab4130-2fd5-4ff7-bbf3-b15120ef706e",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}