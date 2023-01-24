{
  "id": "65",
  "name": "Buffer Overflow: The attacker crafts the content to be injected.",
  "description": "If the intent is to simply cause the software to crash, the content need only consist of an excessive quantity of random data.\n\n If the intent is to leverage the overflow for execution of arbitrary code, the attacker will craft a set of content that not only overflows the targeted buffer but does so in such a way that the overwritten return address is replaced with one of the attackers&#39; choosing which points to code injected by the attacker.\n\nReference: https://capec.mitre.org/data/definitions/100.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "c74ac615-da8a-450c-b85a-7b6cb1cf8fb9",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}