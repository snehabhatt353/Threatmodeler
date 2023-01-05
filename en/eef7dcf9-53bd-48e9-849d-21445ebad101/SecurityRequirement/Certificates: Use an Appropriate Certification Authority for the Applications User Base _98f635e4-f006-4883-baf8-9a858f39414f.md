{
  "id": "62",
  "name": "Certificates: Use an Appropriate Certification Authority for the Applications User Base ",
  "description": "An application user must never be presented with a warning that the certificate was signed by an unknown or untrusted authority. The application's user population must have access to the public certificate of the certification authority which issued the server's certificate. For Internet accessible websites, the most effective method of achieving this goal is to purchase the TLS certificate from a recognize certification authority. Popular Internet browsers already contain the public certificates of these recognized certification authorities.\n\nInternal applications with a limited user population can use an internal certification authority provided its public certificate is securely distributed to all users. However, remember that all certificates issued by this certification authority will be trusted by the users. Therefore, utilize controls to protect the private key and ensure that only authorized individuals have the ability to sign certificates.\n\nThe use of self signed certificates is never acceptable. Self signed certificates negate the benefit of end-point authentication and also significantly decrease the ability for an individual to detect a man-in-the-middle attack.",
  "labels": "ThreatModeler,AppSec and InfraSec,Certificate Authority,Web Application,Web Service,Web Server,Key Management Server,TM-391",
  "libraryId": "1",
  "isHidden": false,
  "guid": "98f635e4-f006-4883-baf8-9a858f39414f",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:48.12",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}