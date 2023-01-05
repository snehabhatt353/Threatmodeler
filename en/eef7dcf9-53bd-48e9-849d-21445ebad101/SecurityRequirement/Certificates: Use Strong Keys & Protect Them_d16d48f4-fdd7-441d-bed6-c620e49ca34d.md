{
  "id": "68",
  "name": "Certificates: Use Strong Keys & Protect Them",
  "description": "<p>The private key used to generate the cipher key must be sufficiently strong for the anticipated lifetime of the private key and corresponding certificate. The current best practice is to select a key size of at least 2048.</p><p>Additional information on key lifetimes and comparable key strengths can be found in NIST SP 800-57. In addition, the private key must be stored in a location that is protected from unauthorized access.</p><p>The algorithms specified in NIST standards (e.g., AES, TDEA, SHA-2, and DSA) and the cryptographic modules in which they reside have required conformance tests. Accredited laboratories perform these tests on vendor implementations that claim conformance to the standards. Vendors are permitted to modify non-conforming implementations so that they meet all applicable requirements. Users of validated implementations can have a high degree of confidence that validated implementations conform to the standards. Since 1977, NIST has developed a cryptographic “toolkit” of NIST standards1 that form a basis for the implementation of approved cryptography. This Recommendation references many of those standards, and provides guidance on how they may be properly used to protect sensitive information.</p><p><br /></p><p><b>Reference:</b></p><p><a href=\"https://cheatsheetseries.owasp.org/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html#use-strong-keys-and-protect-them\" target=\"_blank\">https://cheatsheetseries.owasp.org/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html#use-strong-keys-and-protect-them</a></p><p><a href=\"https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57pt1r4.pdf\" target=\"_blank\">https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57pt1r4.pdf</a></p><p><br /></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Web Server,Web Application,Web Service,Database,SQL Database,TM-513",
  "libraryId": "1",
  "isHidden": false,
  "guid": "d16d48f4-fdd7-441d-bed6-c620e49ca34d",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-09T14:31:41.71",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}