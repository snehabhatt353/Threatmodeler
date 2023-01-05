{
  "id": "101",
  "name": "Remote File Inclusion prevention",
  "description": "<p>A remote file inclusion (RFI) occurs when a file from a remote web server is inserted into a web page. This can be done on purpose to display content from a remote web application. But, it can also happen by accident, due to a misconfiguration of the respective programming language, which can lead to a RFI attack.</p><p>Even though this kind of file inclusion can occur in almost every kind of web application, those written in PHP code are more likely to to be vulnerable to Remote File Inclusion attacks, because PHP provides native functions that allow the inclusion of remote files. Other languages usually require a workaround to imitate this behavior.</p><p>In order to include a remote file you have to add a string with the url of the file to an Include function of the respective language (for example, PHP). Then the web server of the website under attack makes a request to the remote file, fetches its contents and includes it on the web page serving the content. It is then processed by the parser of the language.</p><p><br /></p><p><b>Implementation:</b></p><p>Validate all input for content including files. Ensure that if files and remote content must be accepted that once accepted, they are placed in a sandbox type location so that lower assurance clients cannot write up to higher assurance processes (like Web server processes for example).</p><p><br /></p><p><b>Reference:</b></p><p><a href=\"https://capec.mitre.org/data/definitions/23.html\" target=\"_blank\">https://capec.mitre.org/data/definitions/23.html</a><a target=\"_blank\" href=\"https://capec.mitre.org/data/definitions/23.html\"></a></p><p><a href=\"https://www.netsparker.com/blog/web-security/remote-file-inclusion-vulnerability/\" target=\"_blank\">https://www.netsparker.com/blog/web-security/remote-file-inclusion-vulnerability/</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,File Server,Web Application,Native Application,TM-180",
  "libraryId": "1",
  "isHidden": false,
  "guid": "490a6aa6-3d19-41d3-aef4-ed2472d26aea",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-16T19:28:41.953",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}