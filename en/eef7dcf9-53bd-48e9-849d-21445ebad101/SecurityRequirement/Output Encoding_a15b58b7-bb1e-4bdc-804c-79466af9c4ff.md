{
  "id": "105",
  "name": "Output Encoding",
  "description": "\"Escaping\" is a technique used to ensure that characters are treated as data, not as characters that are relevant to the interpreter's parser. There are lots of different types of escaping, sometimes confusingly called output \"encoding.\" Some of these techniques define a special \"escape\" character, and other techniques have a more sophisticated syntax that involves several characters.\n\nEscaping is the primary means to make sure that untrusted data can't be used to convey an injection attack. There is no harm in escaping data properly - it will still render in the browser properly. Escaping simply lets the interpreter know that the data is not intended to be executed, and therefore prevents attacks from working.\n\n\nExamples using OWASP ESAPI:\n\nFirst, a simple example to output to an HTML entity.\n\n//performing input validation\nString cleanComment = ESAPI.validator().getValidInput(\"comment\",\nrequest.getParameter(\"comment\"), \"CommentRegex\", 300, false, errorList);\n\n//check the errorList here ...\n...\n\n//performing output encoding for the HTML context\nString safeOutput = ESAPI.encoder().encodeForHTML( cleanComment );\n\n\n\n\nNow, an example of creating a URL that is safe for output.\n\n//performing input validation\nString cleanUserName = ESAPI.validator().getValidInput(\"userName\",\nrequest.getParameter(\"userName\"), \"userNameRegex\", 50, false, errorList);\n\n//check the errorList here ...\n...\n\n//performing output encoding for the url context\nString safeOutput = \"/admin/findUser.do?name=\"\n+ ESAPI.encoder().encodeForURL(cleanUserName);\n\nReference: https://www.owasp.org/index.php/Injection_Theory ",
  "labels": "ThreatModeler,AppSec and InfraSec,Web Application,Web Service,Web Browser,API,TM-416",
  "libraryId": "1",
  "isHidden": false,
  "guid": "a15b58b7-bb1e-4bdc-804c-79466af9c4ff",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:49.233",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}