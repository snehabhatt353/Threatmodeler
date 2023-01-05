{
  "id": "97",
  "name": "Predefined list for reflection utilizing external input",
  "description": "<p>If it is necessary to allow reflection utilizing external input, limit the possible values to a predefined list. For example, reflection is commonly used for loading JDBC database connector classes. Most often, the string class name is read from a configuration file. </p><p>Injection problems can be avoided by embedding a list of strings naming each of the supported database driver classes and requiring the class name read from the file to be in the list before loading.</p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Web Application,Web Service,TM-249",
  "libraryId": "1",
  "isHidden": false,
  "guid": "6680e7e1-c689-4334-bce1-c8206ec42973",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:49.077",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}