{
  "id": "103",
  "name": "Host Integrity Checking",
  "description": "<p>Host Integrity (HI) is a feature of Symantec Endpoint Protection (SEP) that can be used to ensure that client computers are protected and compliant with a company's security policies.  Host Integrity policies can used to define, enforce, and remediate the security of clients as defined by the policy.  For example, an HI policy can be used to check if a specific Microsoft patch, or set of patches are installed on a client.  If a client fails to meet the requirements, the client can be quarantined from certain network access until the client meets those requirements.</p><p>The Requirements section has two sections: When you want HI checks to run and the HI Requirements.  Clicking the Add button towards the bottom of the page brings up the Add Requirement Wizard.  To check if a specific Microsoft patch is installed you can use two different options: Patch requirement and Custom requirement.</p><ul><li>Patch requirement - Simple requirement useful for checking a single patch per requirement. <br /></li><li>Custom Requirement - Better suited for checking for the presence of one patch out of a set of patches.  </li></ul><p>Example:  A CVE is addressed in a Microsoft Security Update and Monthly Rollup.  The Security Update and Monthly Rollup have different KB numbers and having either installed address the CVE.  A Patch Requirement can only only check against one Patch Name and return a PASS/FAIL, whereas a Custom Requirement can use OR logic to determine if either of the KBs are installed.</p><p>Host integrity monitoring for critical files, directories, and processes. The goal of host integrity monitoring is to be aware when a security issue has occurred so that incident response and other forensic activities can begin.</p><p><br /></p><p>To configure a Host Integrity policy</p><ol><li>Log into the Symantec Endpoint Protection Manager (SEPM).</li><li>Click on Policies.</li><li>Select Host Integrity on the left.</li><li>Select the desired HI policy, then edit it.</li></ol><p><br /></p><p><b>Reference:</b></p><p><a href=\"https://knowledge.broadcom.com/external/article/179348/using-endpoint-protections-host-integrit.html\" target=\"_blank\">https://knowledge.broadcom.com/external/article/179348/using-endpoint-protections-host-integrit.html</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,File,File System,Operating System,OS Process,TM-582",
  "libraryId": "1",
  "isHidden": false,
  "guid": "eea0ce27-1996-45b1-8128-7cd1c448ad83",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-09-29T15:34:56.57",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}