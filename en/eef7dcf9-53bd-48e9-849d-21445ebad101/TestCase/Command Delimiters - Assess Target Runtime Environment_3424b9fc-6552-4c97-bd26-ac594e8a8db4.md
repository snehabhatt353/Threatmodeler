{
  "id": "106",
  "name": "Command Delimiters - Assess Target Runtime Environment",
  "description": "In situations where the runtime environment is not implicitly known, the attacker makes connections to the target system and tries to determine the system's runtime environment. Knowing the environment is vital to choosing the correct delimiters.\n\nAttack Step Techniques:\n1.   Port mapping using network connection-based software (e.g., nmap, nessus, etc.)\nenv-ClientServer env-Embedded env-CommProtocol env-Peer2Peer env-Web\n\n2.   Port mapping by exploring the operating system (netstat, sockstat, etc.)\nenv-Local\n\n3.   TCP/IP Fingerprinting\nenv-All\n\n4.   Induce errors to find informative error messages\nenv-All\n\nIndicators: \n1.   Positive,   The target software accepts connections via the network.\nenv-Web env-CommProtocol env-Peer2Peer env-Embedded\n\nOutcomes:\n1.   Success,   Operating environment (operating system, language, and/or middleware) is correctly identified.\n2.   Inconclusive,   Multiple candidate operating environments are suggested.\n\nSecurity Controls:\n1.   Preventative,   Provide misleading information on TCIP/IP fingerprints (some operating systems can be configured to send signatures that match other operating systems).\n2.  Preventative,   Provide misleading information at the server level (e.g., Apache, IIS, WebLogic, etc.) to announce a different server software.\n3.   Detective,   Some fingerprinting techniques can be detected by operating systems or by network IDS systems because they leave the network connection half-open, or they do not belong to a valid, open connection.\n\nReference:https://capec.mitre.org/data/definitions/15.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "3424b9fc-6552-4c97-bd26-ac594e8a8db4",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}