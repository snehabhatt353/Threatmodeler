{
  "id": "59",
  "name": "TLS: Prevent Caching of Sensitive Data",
  "description": "<p>Failure frequently compromises all data that should have been protected. Typically, this information includes sensitive personal information (PII) data such as health records, credentials, personal data, and credit cards, which often require protection as defined by laws or regulations such as the EU GDPR or local privacy laws.</p><p>Although TLS provides protection of data while it is in transit, it does not provide any protection for data once it has reached the requesting system. As such, this information may be stored in the cache of the user's browser, or by any intercepting proxies which are configured to perform TLS decryption.</p><p>Where sensitive data is returned in responses, HTTP headers should be used to instruct the browser and any proxy servers not to cache the information, in order to prevent it being stored or returned to other users. This can be achieved by setting the following HTTP headers in the response:</p><p>Cache-Control: no-cache, no-store, must-revalidate</p><p>Pragma: no-cache</p><p>Expires: 0</p><p><br /></p><p><b>Implementation:</b></p><ul><li>Ensure up-to-date and strong standard algorithms, protocols, and keys are in place; use proper key management.</li><li>Encrypt all data in transit with secure protocols such as TLS with perfect forward secrecy (PFS) ciphers, cipher prioritization by the server, and secure parameters. Enforce encryption using directives like HTTP Strict Transport Security (HSTS).</li><li>Disable caching for response that contain sensitive data.</li></ul><p><br /></p><p>Reference:</p><p><a href=\"https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A3-Sensitive_Data_Exposure\" target=\"_blank\">https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A3-Sensitive_Data_Exposure</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,TLS,TM-122",
  "libraryId": "1",
  "isHidden": false,
  "guid": "2ef6e8ab-b4b6-4054-83b3-1e4c2d0c5b60",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-09-29T15:34:56.54",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}