{
  "id": "133",
  "name": "Redirect Access to Libraries - Craft malicious libraries",
  "description": "The attacker uses knowledge gained in the Explore phase to craft malicious libraries that he will redirect the target to leverage. These malicious libraries could have the same APIs as the legitimate library and additional malicious code.\n\nAttack Step Techniques:\n1\tThe attacker monitors the file operations performed by the target application using a tool like dtrace or FileMon. And the attacker can delay the operations by using \"sleep(2)\" and \"usleep()\" to prepare the appropriate conditions for the attack, or make the application perform expansive tasks (large files parsing, etc.) depending on the purpose of the application.\nenv-Local\n\nOutcomes:\n1\tSuccess\t\nThe entries in the configuration file points to the malicious libraries he crafted.\n\nSecurity Controls:\n1\tPreventative\t\nRestrict the permission to modify the entries in the configuration file.\n2\tPreventative\t\nIf possible, use obfuscation and other techniques to prevent reverse engineering the libraries.\n\nReference: https://capec.mitre.org/data/definitions/159.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "b630abe4-b0a5-46c7-aafe-f8418e25fa17",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}