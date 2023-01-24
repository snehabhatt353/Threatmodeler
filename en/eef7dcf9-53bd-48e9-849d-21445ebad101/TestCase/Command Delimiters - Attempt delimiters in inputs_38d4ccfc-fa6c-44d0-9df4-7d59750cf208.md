{
  "id": "108",
  "name": "Command Delimiters - Attempt delimiters in inputs",
  "description": "The attacker systematically attempts variations of delimiters on known inputs, observing the application's response each time.&nbsp; Attack Step Techniques 1. Inject command delimiters using network packet injection tools (netcat, nemesis, etc.) env-CommProtocol env-Web env-Peer2Peer env-ClientServer 2. Inject command delimiters using web test frameworks (proxies, TamperData, custom programs, etc.) env-Web 3. Enter command delimiters directly in input fields. env-Embedded env-Local env-ClientServer Indicators: 1. Positive, Attack step 2 is successful. env-All Outcomes 1.\tSuccess, One or more command delimiters for the platform provokes an unexpected response from the software, which can be varied by the attacker based on the input. Reference: https://capec.mitre.org/data/definitions/15.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "38d4ccfc-fa6c-44d0-9df4-7d59750cf208",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}