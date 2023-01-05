{
  "id": "141",
  "name": "Legitimate HTTP Verbs",
  "description": "<p>HTTP Verb Tampering is an attack that exploits vulnerabilities in HTTP verb (also known as HTTP method) authentication and access control mechanisms. Many authentication mechanisms only limit access to the most common HTTP methods, thus allowing unauthorized access to restricted resources by other HTTP methods.</p><p>Many Web server authentication mechanisms use verb-based authentication and access controls. Such security mechanisms include access control rules for requests with specific HTTP methods. For example, an administrator can configure a Web server to allow unrestricted access to a Web page using HTTP GET requests, but restrict POSTs to administrators only. However, many implementations of verb-based security mechanisms enforce the security rules in an unsecure manner, allowing access to restricted resources by using alternative HTTP methods (such as HEAD) or even arbitrary character strings.<br /></p><p>Ensure that only legitimate HTTP verbs are allowed. Verb tampering attacks exploit either configuration flaws in the access control mechanism or vulnerabilities in the request handlers’ code. As presented in the example above, blocking requests that use non-standard HTTP methods is not enough because in many cases an attacker can use a legitimate HTTP method like HEAD.<br /></p><p><br /></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,HTTP,HTTPS,TM-303",
  "libraryId": "1",
  "isHidden": false,
  "guid": "78500cbd-5634-495a-b68b-aebd9af7854b",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-17T13:57:30.18",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}