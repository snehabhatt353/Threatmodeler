{
  "id": "81",
  "name": "Cross Site Tracing- Create a malicious script that pings the web server with HTTP TRACE request:",
  "description": "Create a malicious script that will induce the victim&#39;s browser to issue an HTTP TRACE request to the destination system&#39;s web server. The script will further intercept the response from the web server, pick up sensitive information out of it, and forward to the site controlled by the attacker.\n\nAttack Step Techniques:\n1.   The attacker&#39;s malicious script circumvents the httpOnly cookie attribute that prevents from hijacking the victim&#39;s session cookie directly using document.cookie and instead leverages the HTTP TRACE to catch this information from the header of the HTTP request once it is echoed back from the web server in the body of the HTTP TRACE response. \n\nReference: https://capec.mitre.org/data/definitions/107.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "bd023aae-85eb-47ce-9469-f8366ad63419",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}