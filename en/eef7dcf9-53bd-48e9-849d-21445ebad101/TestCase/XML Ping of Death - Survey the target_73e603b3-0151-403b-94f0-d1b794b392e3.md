{
  "id": "130",
  "name": "XML Ping of Death - Survey the target",
  "description": "Using a browser or an automated tool, an attacker records all instance of web services to process XML requests.\nAttack Step Techniques:\n1\tUse an automated tool to record all instances of URLs to process XML requests.\nenv-Web env-ClientServer\n2\tUse a browser to manually explore the website and analyze how the application processes XML requests.\nenv-Web env-ClientServer\n\nIndicators:\n1\tPositive\t\nThe URL processes XML requests.\nenv-Web env-ClientServer\n2\tPositive\t\nThe application does not accept XML requests.\nenv-Web env-ClientServer\n\nOutcomes:\n1\tSuccess\t\nA list of URLs which process XML requests.\n\nSecurity Controls:\n1\tDetective\t\nMonitor velocity of page fetching in web logs. Humans who view a page and select a link from it will click far slower and far less regularly than tools. Tools make requests very quickly and the requests are typically spaced apart regularly (e.g. 0.8 seconds between them).\n\nReference: https://capec.mitre.org/data/definitions/147.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "73e603b3-0151-403b-94f0-d1b794b392e3",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}