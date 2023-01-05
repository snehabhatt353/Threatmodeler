{
  "id": "79",
  "name": "Minimize vulnerabilities at web document root level.",
  "description": "<p>Store library, include, and utility files outside of the web document root, if possible. </p><p>Properly controlling access to web content is crucial for running a secure web server. Directory traversal or Path Traversal is an HTTP attack which allows attackers to access restricted directories and execute commands outside of the web server’s root directory.<div>Web servers provide two main levels of security mechanisms</div><div>• Access Control Lists (ACLs)</div><div>• Root directory</div><div><br /></div><div>With a system vulnerable to directory traversal, an attacker can make use of this vulnerability to step out of the root directory and access other parts of the file system. This might give the attacker the ability to view restricted files, which could provide the attacker with more information required to further compromise the system.</div><div>Depending on how the website access is set up, the attacker will execute commands by impersonating himself as the user which is associated with “the website”. Therefore it all depends on what the website user has been given access to in the system.</div><div><br /></div><div><b>Implementation:</b></div><div><b><br /></b>First of all, ensure you have installed the latest version of your web server software, and sure that all patches have been applied.</div><div>Secondly, effectively filter any user input. Ideally remove everything but the known good data and filter meta characters from the user input. This will ensure that only what should be entered in the field will be submitted to the server.</div><div><br /></div><div>Reference:</div><div><a href=\"https://www.beyondtrust.com/blog/entry/what-is-least-privilege\" target=\"_blank\">https://www.beyondtrust.com/blog/entry/what-is-least-privilege</a></div></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Web Server,Host,TM-525",
  "libraryId": "1",
  "isHidden": false,
  "guid": "d4f9d490-1acc-4538-baca-89a6d15d12c0",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-09T14:35:03.157",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}