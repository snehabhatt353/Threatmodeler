{
  "id": "72",
  "name": "Certificates: Always Provide All Needed Certificates ",
  "description": "<p>When a user receives a server or host's certificate, the certificate must be validated back to a trusted root certification authority. This is known as path validation.\n\nThere can be one or more intermediate certificates in between the end-entity (server or host) certificate and root certificate. </p><p>In addition to validating both endpoints, the user will also have to validate all intermediate certificates. Validating all intermediate certificates can be tricky because the user may not have them locally. This is a well-known PKI issue called the “Which Directory?\" problem.\n\n</p><p>To avoid the “Which Directory?\" problem, a server should provide the user with all required certificates used in a path validation.</p>",
  "labels": "",
  "libraryId": "1",
  "isHidden": false,
  "guid": "da924477-3ca1-4248-85fb-c563e8ca0425",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:48.37",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}