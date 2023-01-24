{
  "id": "83",
  "name": "Command Line Execution through SQL Injection Test Case",
  "description": "<p><strong>Explore</strong></p><p><strong></strong>Probe for SQL Injection vulnerability: The attacker injects SQL syntax into user-controllable data inputs to search unfiltered execution of the SQL syntax in a query.</p><p></p><p><strong>Exploit</strong></p><p><strong></strong>Achieve arbitrary command execution through SQL Injection with the MSSQL_xp_cmdshell directive: The attacker leverages a SQL Injection attack to inject shell code to be executed by leveraging the xp_cmdshell directive.</p><p>Inject malicious data in the database: Leverage SQL injection to inject data in the database that could later be used to achieve command injection if ever used as a command line argument</p><p>Trigger command line execution with injected arguments: The attacker causes execution of command line functionality which leverages previously injected database content as arguments.</p>",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "3a847071-0427-4a54-bb93-4b4729b16b4c",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}