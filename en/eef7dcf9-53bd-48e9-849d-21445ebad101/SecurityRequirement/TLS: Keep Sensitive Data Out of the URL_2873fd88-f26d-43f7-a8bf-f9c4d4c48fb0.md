{
  "id": "58",
  "name": "TLS: Keep Sensitive Data Out of the URL",
  "description": "<p>Sensitive data must not be transmitted via URL arguments. A more appropriate place is to store sensitive data in a server side repository or within the user's session. When using TLS the URL arguments and values are encrypted during transit. However, there are two methods that the URL arguments and values could be exposed.\n</p><p>\n1. The entire URL is cached within the local user's browser history. This may expose sensitive data to any other user of the workstation.\n</p><p>\n2. The entire URL is exposed if the user clicks on a link to another HTTPS site. This may expose sensitive data within the referral field to the third party site. This exposure occurs in most browsers and will only occur on transitions between two TLS sites.\n</p><p>\nFor example, a user following a link on https://example.com which leads to https://someOtherexample.com would expose the full URL of https://example.com (including URL arguments) in the referral header (within most browsers). This would not be the case if the user followed a link on https://example.com to http://someHTTPexample.com</p><p>URLs can be cached in a client's browser history or application logs and sent to another HTTPS site if the user clicks on a link. Setting TLS pages to be uncacheable prevents information leakage from the client cache</p><p><br /></p><p><b>Implementation:</b></p><p>Ensure browsers and applications only access your site via HTTPS by enacting HTTP Strict Transport Security (HSTS). Servers utilizing HSTS send an HTTPS header in their response specifying that requests to their domain should only use HTTPS. An HSTS-complaint client should then make all future requests to that domain over HTTPS, even if HTTP is specified. This helps protect clients from man-in-the-middle and eavesdropping attacks that could be initiated by the client sending sensitive information by making an unsecure HTTP request.</p><p><br /></p><p><b>Reference:</b></p><p><a target=\"_blank\" href=\"https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A3-Sensitive_Data_Exposure\">https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A3-Sensitive_Data_Exposure</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,URL,TLS,SSL,TM-101",
  "libraryId": "1",
  "isHidden": false,
  "guid": "2873fd88-f26d-43f7-a8bf-f9c4d4c48fb0",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-02T19:26:47.667",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}