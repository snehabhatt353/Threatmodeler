{
  "id": "88",
  "name": "Email Header Validation",
  "description": "<p>Perform validation on email header data. It is common practice for web pages and web applications to implement contact forms, which in turn send email messages to the intended recipients. Most of the time, such contact forms set headers. These headers are interpreted by the email library on the web server and turned into resulting SMTP commands, which are then processed by the SMTP server.</p><p>Unfortunately, user input is often not validated before being sent to the email library. In such cases, the contact form might be vulnerable to email header injection (also referred to as SMTP header injection or simply email injection). A malicious user may be able to introduce additional headers into the message, thereby instructing the mail server to behave differently than intended.<br /></p><p>Email Injection is not directly dangerous to the owner of the web server, but a vulnerable contact form may be used for sending spam or for phishing. This makes it a serious application security vulnerability.</p><p><br /></p><p><b>Implementation:</b></p><p>To avoid header injection vulnerabilities as well as many other vulnerabilities, the programmer must never trust any user input. Mitigating against email header injection involves validating user input. You must not allow any newline characters in the input because they let the attacker append email headers. In general, when validating user input, the simplest and most robust way to achieve strong input validation is through a whitelist of allowed characters.</p><p><br /></p><p><b>Reference:</b></p><p><a href=\"https://www.acunetix.com/blog/articles/email-header-injection/\" target=\"_blank\">https://www.acunetix.com/blog/articles/email-header-injection/</a></p><p />",
  "labels": "ThreatModeler,AppSec and InfraSec,Email Server,TM-330",
  "libraryId": "1",
  "isHidden": false,
  "guid": "8309354a-daca-48fd-a40c-76b2eaf10ece",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-11T16:31:24.067",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}