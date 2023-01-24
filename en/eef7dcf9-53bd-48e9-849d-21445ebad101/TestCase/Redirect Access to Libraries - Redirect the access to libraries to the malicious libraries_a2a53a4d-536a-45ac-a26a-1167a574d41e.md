{
  "id": "134",
  "name": "Redirect Access to Libraries - Redirect the access to libraries to the malicious libraries",
  "description": "The attacker redirects the target to the malicious libraries he crafted in the Experiment phase. The attacker will be able to force the targeted application to execute arbitrary code when the application attempts to access the legitimate libraries.\nAttack Step Techniques\nID\tAttack Step Technique Description\tEnvironments\tLeveraged Attack Patterns\n1\t\nThe attacker modifies the entries in the configuration files pointing to the malicious libraries he crafted.\nenv-Local\n2\t\nThe attacker leverages symlink/timing issues to redirect the target to access the malicious libraries he crafted.\nenv-Local\n132\n3\t\nThe attacker leverages file search path order issues to redirect the target to access the malicious libraries he crafted.\nenv-Local\n38\nOutcomes\nID\tType\tOutcome Description\n1\tSuccess\t\nThe application is redirected to the malicious libraries the attacker crafted when the application attempts to call the legitimate libraries.\nSecurity Controls\nID\tType\tSecurity Control Description\n1\tPreventative\t\nRestrict the permission to modify the entries in the configuration file.\n2\tPreventative\t\nCheck the integrity of the dynamically linked libraries before using them.\n3\tPreventative\t\nIf possible, use obfuscation and other techniques to prevent reverse engineering the libraries.\n\nReference: https://capec.mitre.org/data/definitions/159.html\n",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "a2a53a4d-536a-45ac-a26a-1167a574d41e",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}