{
  "id": "62",
  "name": "ORM Injection - Probe for ORM Injection vulnerabilities",
  "description": "The attacker injects ORM syntax into user-controllable data inputs of the application to determine if it is possible modify data query structure and content.\n\nIndicators:\n1. (Negative)\t  Attacker receives normal response from server.\nenv-Web env-ClientServer env-Peer2Peer env-CommProtocol\n\n2. (Positive)\t Attacker receives an error message from server indicating that there was a problem with the data query.\nenv-Web env-ClientServer env-Peer2Peer env-CommProtocol\n\n3. (Negative)\t  Server sends a specific error message that indicates programmatic parsing of the input data (e.g. NumberFormatException)\nenv-Web env-ClientServer env-Peer2Peer env-CommProtocol\n\n\nRefrenece: https://capec.mitre.org/data/definitions/109.html ",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "af761ba8-636f-4f97-b485-9bb1f37aa75c",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}