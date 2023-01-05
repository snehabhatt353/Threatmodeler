{
  "id": "116",
  "name": "Disable default database functionality",
  "description": "<p>It is important to develop a security policy for every database. The security policy establishes methods for protecting your database from accidental or malicious destruction of data or damage to the database infrastructure.</p><p>Each database can have an administrator, referred to as the security administrator, who is responsible for implementing and maintaining the database security policy If the database system is small, the database administrator can have the responsibilities of the security administrator. However, if the database system is large, a designated person or group of people may have sole responsibility as security administrator.</p><p><br /></p><p><b>Mitigation:</b></p><p>By far the most effective way to prevent OS command injection vulnerabilities is to never call out to OS commands from application-layer code. In virtually every case, there are alternate ways of implementing the required functionality using safer platform APIs. </p><p>If it is considered unavoidable to call out to OS commands with user-supplied input, then strong input validation must be performed. Some examples of effective validation include: </p><ul><li>Validating against a whitelist of permitted values. </li><li>Validating that the input is a number. </li><li>Validating that the input contains only alphanumeric characters, no other syntax or whitespace. </li><li>Never attempt to sanitize input by escaping shell metacharacters. In practice, this is just too error-prone and vulnerable to being bypassed by a skilled attacker.</li><li>Disable MSSQL xp_cmdshell directive on the database.</li></ul><p><br /></p><p><b>Reference:</b></p><p><a href=\"https://portswigger.net/web-security/os-command-injection\" target=\"_blank\">https://portswigger.net/web-security/os-command-injection</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Database,SQL Database,TM-172",
  "libraryId": "1",
  "isHidden": false,
  "guid": "45cd25c2-e61e-47ff-90ad-094e4106dfc4",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-10T18:05:33.777",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}