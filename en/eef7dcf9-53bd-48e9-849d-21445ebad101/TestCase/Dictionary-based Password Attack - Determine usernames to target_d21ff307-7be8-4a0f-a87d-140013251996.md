{
  "id": "112",
  "name": "Dictionary-based Password Attack - Determine usernames to target",
  "description": "Determine username(s) whose passwords to crack.\n\nAttack Step Techniques:\n1.    Obtain username(s) by sniffing network packets.\nenv-CommProtocol env-Peer2Peer env-ClientServer\n\n2.    Obtain username(s) by querying application/system (e.g. if upon a failed login attempt, the system indicates whether the entered username was valid or not)\nenv-All\n\n3.   Obtain usernames from filesystem (e.g. list of directories in C:\\Documents and Settings\\ in Windows, and list in /etc/passwd in UNIX-like systems)\nenv-Embedded env-Local\n\nIndicators:\n1.   Negative,   Remote application or system provides no indication regarding whether a given username is valid or not.\nenv-ClientServer env-Peer2Peer env-Web env-CommProtocol\n\nOutcomes:\n1.   Success,   At least one valid username found.\n2.   Failure,   Presence of any valid usernames could not be established.\n\nSecurity Controls: \n1\tPreventative,   Do not reveal information regarding validity of particular usernames to users.\n2\tCorrective, Lock out accounts whose usernames are suspected to have been compromised.\n\nReference: https://capec.mitre.org/data/definitions/16.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "d21ff307-7be8-4a0f-a87d-140013251996",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}