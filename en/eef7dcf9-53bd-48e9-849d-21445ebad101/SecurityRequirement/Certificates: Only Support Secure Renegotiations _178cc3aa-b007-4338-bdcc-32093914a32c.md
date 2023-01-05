{
  "id": "66",
  "name": "Certificates: Only Support Secure Renegotiations ",
  "description": "<p>A flaw in the design of the <b>TLS v. 1/SSL v. 3 </b>(TLS/SSL) handshake process was discovered in 2009, and RFC 5746 (Feb. 2010) was released to update the protocol specification. Since then, most system manufacturers have released patches to fix this flaw. Still, as of 2020 approximately half of the systems using TLS/SSL on the Internet have not implemented the patches needed to close this security hole. </p><p>This vulnerability affects the secure transport of HTTP, IMAP, SMTP, and other protocols that rely on TLS/SSL. Industry representatives and security researchers who have looked into the problem note that sites with the TLS patch may still be vulnerable to this attack, known as the TLS renegotiation Man-In-The-Middle attack (<b>TLS Renego MITM</b>).<br><br>Server administrators should <b>disable SSL version 2</b> and <b>disallow the use of weak cipher suites. </b></p><p><br></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,HTTPS,TLS,SSL,Certificate Authorities,IMAP,SMTP,TM-55",
  "libraryId": "1",
  "isHidden": false,
  "guid": "178cc3aa-b007-4338-bdcc-32093914a32c",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:48.277",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}