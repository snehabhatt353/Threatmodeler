{
  "id": "106",
  "name": "Output Validation",
  "description": "<p>The data needs to be validated from the sources coming from remote users which is similar to input validation</p><p>If script code either does not properly validate input, or does not perform proper output encoding, thus creating an opportunity for an adversary to inject a malicious script launch a XSS attack. A key distinction between other XSS attacks and DOM-based attacks is that in other XSS attacks, the malicious script runs when the vulnerable web page is initially loaded, while a DOM-based attack executes sometime after the page loads. Another distinction of DOM-based attacks is that in some cases, the malicious script is never sent to the vulnerable web server at all. An attack like this is guaranteed to bypass any server-side filtering attempts to protect users.</p><p><br /></p><p><b>Output validation can be performed similarly to input validation like:</b></p><ul><li>Whitelisting vs blacklisting</li><li>Validating free-form Unicode text</li><li>Regular expressions</li></ul><p>Perform output validation for all remote content.</p><p><br /></p><p><b>Reference:</b></p><p><a target=\"_blank\" href=\"https://capec.mitre.org/data/definitions/588.html\">https://capec.mitre.org/data/definitions/588.html</a></p><p><a target=\"_blank\" href=\"https://cheatsheetseries.owasp.org/cheatsheets/Input_Validation_Cheat_Sheet.html#whitelisting-vs-blacklisting\">https://cheatsheetseries.owasp.org/cheatsheets/Input_Validation_Cheat_Sheet.html#whitelisting-vs-blacklisting</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Web Server,Database,SQL Database,TM-551,Web Application,Web Service,Delete,Create,CRUD,Update,Read,Third Party Web Service,Registration",
  "libraryId": "1",
  "isHidden": false,
  "guid": "dff04da5-df90-47c2-9adf-ace626a81346",
  "riskId": 4,
  "isCompensatingControl": false,
  "riskName": "Low",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-12-15T15:56:38.743",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}