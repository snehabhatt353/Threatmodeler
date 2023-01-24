{
  "id": "118",
  "name": "Buffer Overflow in Local Command-Line Utilities - Attacker identifies command utilities exposed by the target host",
  "description": "This attack targets command-line utilities available in a number of shells. An attacker can leverage a vulnerability found in a command-line utility to escalate privilege to root.\r\n\r\n\r\n\r\nExperiment\r\nOn the probing stage, the attacker interacts with the command utility and observes the results of its input. The attacker's goal is to uncover a buffer overflow in the command utility. For instance the attacker may find that input data are not properly validated.\r\nExploit\r\nThe attacker finds a buffer overflow vulnerability in the command utility and tries to exploit it. He crafts malicious code and injects it using the command utility. The attacker can at worst execute remote code on the target host.\r\n\r\n\r\nReference: https://capec.mitre.org/data/definitions/9.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "2773d87d-5d7c-4c50-9f8d-f6972b39ccd3",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}