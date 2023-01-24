{
  "id": "90",
  "name": "JSON Hijacking - Craft a malicious website",
  "description": "The attacker crafts a malicious website to which he plans to lure the victim who is using the vulnerable target system. The malicious website does two things:\n\n    1. Contains a hook that intercepts incoming JSON objects, reads their contents and forwards the contents to the server controlled by the attacker (via a new XMLHttpRequest).\n    2. Uses the script tag with a URL in the source that requests a JSON object from the vulnerable target system. Once the JSON object is transmitted to the victim's browser, the malicious code (as described in step 1) intercepts that JSON object, steals its contents, and forwards to the attacker.\n\nThis attack step leverages the fact that the same origin policy in the browser does not protect JavaScript originating from one domain from setting up an environment to intercept and access JSON objects arriving from a completely different domain.\n\nOutcomes:\n1.   Success,   The JSON object hook captures, reads and forwards JSON objects\n2.   Success,   The malicious website effectively requests JSON objects from the target system\n\nReference: https://capec.mitre.org/data/definitions/111.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "5246969b-f549-4ea1-94a1-5d019d124e60",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}