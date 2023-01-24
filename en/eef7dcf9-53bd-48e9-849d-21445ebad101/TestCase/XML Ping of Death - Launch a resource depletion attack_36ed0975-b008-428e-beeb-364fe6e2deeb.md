{
  "id": "131",
  "name": "XML Ping of Death - Launch a resource depletion attack",
  "description": "The attacker delivers a large number of small XML messages to the target URLs found in the explore phase at a sufficiently rapid rate. It causes denial of service to the target application.\nAttack Step Techniques:\n1\tSend a large number of crafted small XML messages to the target URL.\nenv-Web env-ClientServer\n\nOutcomes:\n1\tSuccess\t\nThe attacker causes the target application denial of service.\n\nSecurity Controls:\n1\tDetective\t\nMonitor velocity of page fetching in web logs.\n2\tPreventative\t\nBuild throttling mechanism into the resource allocation. Provide for a timeout mechanism for allocated resources whose transaction does not complete within a specified interval.\n\nReference: https://capec.mitre.org/data/definitions/147.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "36ed0975-b008-428e-beeb-364fe6e2deeb",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}