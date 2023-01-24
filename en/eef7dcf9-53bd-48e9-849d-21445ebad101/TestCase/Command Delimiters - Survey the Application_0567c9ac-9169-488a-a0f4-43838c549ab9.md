{
  "id": "107",
  "name": "Command Delimiters - Survey the Application",
  "description": "The attacker surveys the target application, possibly as a valid and authenticated user\n\nAttack Step Techniques:\n1.   Spidering web sites for all available links\nenv-Web\n2.   Inventory all application inputs\nenv-All\n\nIndicators:\n1.   Positive,   Attacker develops a list of valid inputs\nenv-Web env-ClientServer\n\nOutcomes:\n1.   Success,   The attacker develops a list of likely command delimiters.\n\nSecurity Controls:\n1.   Detective,   Monitor velocity of page fetching in web logs. Humans who view a page and select a link from it will click far slower and far less regularly than tools. Tools make requests very quickly and the requests are typically spaced apart regularly (e.g. 0.8 seconds between them).\n2.   Detective,   Create links on some pages that are visually hidden from web browsers. Using iframes, images, or other HTML techniques, the links can be hidden from web browsing humans, but visible to spiders and programs. A request for the page, then, becomes a good predictor of an automated tool probing the application.\n\n3.   Preventative,   Actively monitor the application and either deny or redirect requests from origins that appear to be automated.\n4.   Detective,   Monitor velocity of feature activations (non-web software). Humans who activate features (click buttons, request actions, invoke APIs, etc.) will do so far slower and far less regularly than tools. Tools make requests very quickly and the requests are typically spaced apart regularly (e.g. 0.8 seconds between them).\n\nReference: https://capec.mitre.org/data/definitions/15.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "0567c9ac-9169-488a-a0f4-43838c549ab9",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}