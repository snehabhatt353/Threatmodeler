{
  "id": "55",
  "name": "TLS: Do Not Provide Non-TLS Pages for Secure Content",
  "description": "<p>All pages which are available over TLS must not be available over a non-TLS connection. A user may inadvertently bookmark or manually type a URL to a HTTP page (e.g. http://example.com/myaccount) within the authenticated portion of the application. If this request is processed by the application then the response, and any sensitive data, would be returned to the user over the clear text HTTP.</p><p><br /></p><p><b>Implementation:</b></p><p>There are three main use cases that make SSL/TLS a must-have for your website:When you need authentication: Any server can pretend to be your server, hijacking the information that people transmit along the way. SSL/TLS allows you to prove the identity of your server so that people know that you are who you say you are.</p><p>To instill trust: If you’re running an e-commerce site or asking users for the kind of data that’s important to them, you need to engender a sense of trust. Using an SSL/TLS certificate is a visible way of showing visitors that they can trust you and it’s much more effective than anything you could say about yourself.</p><p>When you need to comply with industry standards: In some industries such as the finance industry, you’ll be required to maintain certain base levels of security. There are also Payment Card Industry (PCI) guidelines that you need to adhere to if you want to accept credit card information on your website. And one of those requirements is the use of an SSL/TLS certificate.</p><p><br /></p><p><b>Reference:</b></p><p><a target=\"_blank\" href=\"https://owasp.deteact.com/cheat/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html\">https://owasp.deteact.com/cheat/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,TLS,SSL,TM-89",
  "libraryId": "1",
  "isHidden": false,
  "guid": "2445e78e-fa75-4137-bb25-124074bed7a2",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-02T19:01:45.723",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}