{
  "id": "65",
  "name": "Certificates: Support TLS-PSK and TLS-SRP for Mutual Authentication ",
  "description": "<p>When using a shared secret or password offer TLS-PSK (Pre-Shared Key) or TLS-SRP (Secure Remote Password), which are known as Password Authenticated Key Exchange (PAKEs). TLS-PSK and TLS-SRP properly bind the channel, which refers to the cryptographic binding between the outer tunnel and the inner authentication protocol. </p><p>IANA currently reserves 79 PSK cipher suites and 9 SRP cipher suites.\n\nBasic authentication places the user's password on the wire in the plain text after a server authenticates itself. Basic authentication only provides unilateral authentication. In contrast, both TLS-PSK and TLS-SRP provide mutual authentication, meaning each party proves it knows the password without placing the password on the wire in the plain text.\n</p><p>\nFinally, using a PAKE removes the need to trust an outside party, such as a Certification Authority (CA).</p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Web Server,Web Application,Web Service,Web Browser,TM-412",
  "libraryId": "1",
  "isHidden": false,
  "guid": "a08f7c82-045f-4aa1-b3b7-e48fa97e6fb6",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:48.263",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}