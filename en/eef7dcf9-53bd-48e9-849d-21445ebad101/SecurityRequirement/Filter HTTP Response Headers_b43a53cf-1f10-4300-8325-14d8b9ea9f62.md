{
  "id": "138",
  "name": "Filter HTTP Response Headers",
  "description": "To avoid HTTP Response Splitting, the application must not rely on user-controllable input to form part of its output response stream. Specifically, response splitting occurs due to injection of CR-LF sequences and additional headers. All data arriving from the user and being used as part of HTTP response headers must be subjected to strict validation that performs simple character-based as well as semantic filtering to strip it of malicious character sequences and headers.",
  "labels": "ThreatModeler,AppSec and InfraSec,Web Server,TM-453",
  "libraryId": "1",
  "isHidden": false,
  "guid": "b43a53cf-1f10-4300-8325-14d8b9ea9f62",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:49.627",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}