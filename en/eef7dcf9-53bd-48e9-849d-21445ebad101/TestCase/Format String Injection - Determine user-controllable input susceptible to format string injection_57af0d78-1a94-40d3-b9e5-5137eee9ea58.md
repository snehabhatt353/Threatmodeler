{
  "id": "100",
  "name": "Format String Injection - Determine user-controllable input susceptible to format string injection",
  "description": "Determine the user-controllable input susceptible to format string injection. For each user-controllable input that the attacker suspects is vulnerable to format string injection, attempt to inject formatting characters such as %n, %s, etc.. The goal is to manipulate the string creation using these formatting characters.\n\nAttack Step Techniques:\n1.   Inject probe payload which contains formatting characters (%s, %d, %n, etc.) through input parameters.\nenv-Web\n\nIndicators\n1.   Negative,   Attacker receives normal response from server.\nenv-Web env-Peer2Peer env-CommProtocol env-ClientServer\n\n2.   Positive,   Attacker receives an abnormal message (let's say with a partial dump of the memory) from the application which indicates that the format string was successfully manipulated.\nenv-Web env-Peer2Peer env-CommProtocol env-ClientServer\n\nOutcomes:\n1.   Success,  At least one user-controllable input susceptible to injection found.\n2.    Failure,   No user-controllable input susceptible to injection found.\n\nSecurity Controls\n1.  Detective,   Search for and report format string injection indicators such as the use of %s, %n, %d, etc. in submitted user input\n2.   Preventative,   Refrain from using format strings when not necessary, for example fprintf(str) can be replaced by fputs(str), etc.\n\n\nReference: https://capec.mitre.org/data/definitions/135.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "57af0d78-1a94-40d3-b9e5-5137eee9ea58",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}