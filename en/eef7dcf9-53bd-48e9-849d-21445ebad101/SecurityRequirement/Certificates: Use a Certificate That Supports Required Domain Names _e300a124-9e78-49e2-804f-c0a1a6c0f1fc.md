{
  "id": "69",
  "name": "Certificates: Use a Certificate That Supports Required Domain Names ",
  "description": "You can secure multiple domains under one certificate, which makes keeping up-to-date with your internet security easy.<br><p>Whether you decide to go for a multi-domain/SAN<sup>1</sup> SSL certificate, a UCC<sup>2</sup> SSL certificate, or a Wildcard certificate will depend on the number of domains and subdomains your business is hosting and whether or not you plan to expand in the future. </p><ul><li>If your multiple domains have a set number of subdomains that you don’t plan on adding to in the future, a multi-domain/SAN certificate is probably the best choice.</li><li> If you have a set number of domains and subdomains in a Microsoft Exchange and Office Communications environment, then UCC certificate is what you should opt for. </li><li>If you only have a single domain and plan on adding more subdomains in the future, you should choose a Wildcard SSL certificate.</li></ul><p>A user should never be presented with a certificate error, including prompts to reconcile domain or host-name mismatches, or expired certificates.<br><br>The presence of certificate errors desensitizes users to TLS error messages and increases the possibility an attacker could launch a convincing phishing or man-in-the-middle attack.<br></p><p><br></p><p><sub>SAN : Subject Alternative Name</sub></p><p><sub>UCC : Unified communications certificates</sub><br><br></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Domain Name Service,URL,TM-560",
  "libraryId": "1",
  "isHidden": false,
  "guid": "e300a124-9e78-49e2-804f-c0a1a6c0f1fc",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:48.293",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}