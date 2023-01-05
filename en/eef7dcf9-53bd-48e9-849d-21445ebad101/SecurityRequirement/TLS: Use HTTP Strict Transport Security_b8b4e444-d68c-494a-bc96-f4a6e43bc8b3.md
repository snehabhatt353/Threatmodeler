{
  "id": "60",
  "name": "TLS: Use HTTP Strict Transport Security",
  "description": "<p>A new browser security setting called HTTP Strict Transport Security (HSTS) will significantly enhance the implementation of TLS for a domain. </p><p>HSTS is enabled via a special response header and this instructs compatible browsers to enforce the following security controls:\nAll requests to the domain will be sent over HTTPS\nAny attempts to send an HTTP requests to the domain will be automatically upgraded by the browser to HTTPS before the request is sent\nIf a user encounters a bad SSL certificate, the user will receive an error message and will not be allowed to override the warning message.</p><p><br /></p><p>HSTS addresses the following threats:</p><p>• User bookmarks or manually types http://example.com and is subject to a man-in-the-middle attacker</p><p>• HSTS automatically redirects HTTP requests to HTTPS for the target domain</p><p>• Web application that is intended to be purely HTTPS inadvertently contains HTTP links or serves content over HTTP</p><p>• HSTS automatically redirects HTTP requests to HTTPS for the target domain</p><p>• A man-in-the-middle attacker attempts to intercept traffic from a victim user using an invalid certificate and hopes the user will accept the bad certificate</p><p>• HSTS does not allow a user to override the invalid certificate messageRecommended:</p><p>• If the site owner would like their domain to be included in the HSTS preload list maintained by Chrome (and used by Firefox and Safari), then use the header below.</p><p>• Sending the preload directive from your site can have PERMANENT CONSEQUENCES and prevent users from accessing your site and any of its subdomains if you find you need to switch back to HTTP. Please read the details at preload removal before sending the header with preload.</p><p>Strict-Transport-Security: max-age=31536000; includeSubDomains; preload</p><p>The preload flag indicates the site owner's consent to have their domain preloaded. The site owner still needs to then go and submit the domain to the list.</p><p><br /></p><p><b>Reference:</b></p><p><a href=\"https://cheatsheetseries.owasp.org/cheatsheets/HTTP_Strict_Transport_Security_Cheat_Sheet.html\" target=\"_blank\">https://cheatsheetseries.owasp.org/cheatsheets/HTTP_Strict_Transport_Security_Cheat_Sheet.html</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Web Server,Web Browser,TM-460",
  "libraryId": "1",
  "isHidden": false,
  "guid": "b8b4e444-d68c-494a-bc96-f4a6e43bc8b3",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-09T14:33:01.03",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}