{
  "id": "92",
  "name": "Limit Privilege by chroot jails",
  "description": "<p>Limit program privileges, so if metacharacters or other methods circumvent program input validation routines and shell access is attained then it is not running under a privileged account. chroot jails create a sandbox for the application to execute in, making it more difficult for an attacker to elevate privilege even in the case that a compromise has occurred.</p><p>Limit program privileges, so if commands circumvent program input validation or filter routines then commands do not running under a privileged account.</p><p><br /></p><p><b>It can be implemented in the following ways by:<br /></b></p><ul><li>Minimize the Privileges Granted</li><li>Minimize the Time the Privilege Can Be Used</li><li>Minimize the Time the Privilege is Active</li><li>Minimize the Modules Granted the Privilege</li><li>Consider Using FSUID To Limit Privileges</li><li>Consider Using Chroot to Minimize Available Files</li><li>Consider Minimizing the Accessible Data</li><li>Consider Minimizing the Resources Available</li></ul><p><br /></p><p><b>Reference:</b></p><p><a target=\"_blank\" href=\"https://www.thegeekdiary.com/understanding-chroot-jail/\">https://www.thegeekdiary.com/understanding-chroot-jail/</a></p><p><a target=\"_blank\" href=\"https://dwheeler.com/secure-programs/Secure-Programs-HOWTO/minimize-privileges.html\">https://dwheeler.com/secure-programs/Secure-Programs-HOWTO/minimize-privileges.html</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,App,Web Application,Native Application,Users,Operating System,Virtual Machine,External System,Account,Web Service,Web Browser,Database,SQL Database,TM-489",
  "libraryId": "1",
  "isHidden": false,
  "guid": "c6fb0196-0419-4c82-b602-8f8398fa9031",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-09T16:56:22.96",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}