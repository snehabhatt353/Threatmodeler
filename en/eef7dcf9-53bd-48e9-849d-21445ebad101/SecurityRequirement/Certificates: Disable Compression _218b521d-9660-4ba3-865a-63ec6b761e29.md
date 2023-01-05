{
  "id": "67",
  "name": "Certificates: Disable Compression ",
  "description": "<p>The <b>CRIME</b> attack makes use of the fact that compression, either on the TLS level or inside the actual protocol wrapped into the TLS session, like HTTP, can reveal details about the contents of the data transferred. </p><p>So even without knowing how to decipher the encrypted return from the server, an attacker can reveal important security tokens like session cookies.<br><br>The only mitigation strategy is disabling compression altogether, for both TLS protocol and web content. It can happen that one tool only reports the TLS compression status, like SSL Labs, another only evaluating web content compression. That’s why the results can diverge. </p><p>Note that in many cases, there are multiple places in different tools where you have to disable compression for – really – getting rid of CRIME: Your load balancer/reverse proxy that usually terminates TLS is one place, another is the tool serving your static files, and finally the application. <br></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Certificate Authorities,TM-84",
  "libraryId": "1",
  "isHidden": false,
  "guid": "218b521d-9660-4ba3-865a-63ec6b761e29",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:48.277",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}