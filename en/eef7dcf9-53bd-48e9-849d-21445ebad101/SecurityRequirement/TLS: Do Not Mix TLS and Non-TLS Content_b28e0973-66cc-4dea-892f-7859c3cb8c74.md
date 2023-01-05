{
  "id": "56",
  "name": "TLS: Do Not Mix TLS and Non-TLS Content",
  "description": "<p>A page that is available over TLS must be comprised completely of content which is transmitted over TLS. The page must not contain any content that is transmitted over unencrypted HTTP. This includes content from unrelated third party sites.\n</p><p>An attacker could intercept any of the data transmitted over the unencrypted HTTP and inject malicious content into the user's page. This malicious content would be included in the page even if the overall page is served over TLS. </p><p>In addition, an attacker could steal the user's session cookie that is transmitted with any non-TLS requests. This is possible if the cookie's 'secure' flag is not set. See the rule 'Use &quot;Secure&quot; Cookie Flag'</p><p><br /></p><p><b>Implementation:</b></p><ul><li>Implement the use of Use the &quot;Secure&quot; Cookie Flag</li><li>Prevent Caching of Sensitive Data</li><li>Use HTTP Strict Transport Security</li><li>Consider the use of Client-Side Certificates</li></ul><p><br /></p><p><b>Reference:</b></p><p><a target=\"_blank\" href=\"https://owasp.deteact.com/cheat/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html\">https://owasp.deteact.com/cheat/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Web Application,TM-449",
  "libraryId": "1",
  "isHidden": false,
  "guid": "b28e0973-66cc-4dea-892f-7859c3cb8c74",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-02T14:52:19.657",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}