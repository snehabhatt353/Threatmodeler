{
  "id": "113",
  "name": "Disable Script Execution",
  "description": "<p>Webroot has discovered ransomware variants delivered through email attachments as well. These malicious attachments are often a zip archive that contain a script, which serves the purpose of downloading/executing a ransomware/malware payload. Webroot recommends preventing the execution of script file types to avoid this type of attack.</p><p>In order to prevent these types of documents and scripts from running we recommend choosing the most appropriate solution for your environment below. </p><p>Block WSF, VBS, WSH, HTA, VBS and JS files.</p><p>If possible, disable script execution in the administrative interface.</p><p><br /></p><p><b>Implementation:</b></p><p>REDIRECT SCRIPT FILE EXTENSIONS VIA GPOTo enable this policy setting, access the system set up for policy control and navigate to the following setting:User Configuration - Preferences - Control Panel - Settings</p><p>Right-click on Folder Options and navigate to New &gt; Open With.Type in the each unwanted extension, i.e. wsf, js, vbs into the &quot;File extension&quot; box, then input the path of a program you want to have as default to open the file.</p><p>Tick Set as default and press OK.Example of redirecting the extension .wsf, .js, and .vbs to notepad:</p><p>We recommend redirecting the file types: .hta, .jse, .js, .vbs, .vbe, .wsf, .wsh, and .ps1.If a system administrator needs to run a WSF, VBS, JS, or any other script file, this can still be achieved by starting the WScript program with the script file as an argument.For example:: C:WindowsSystem32WSCRIPT.exe C:example.vbs</p><p><br /></p><p><b>Reference:</b></p><p><a target=\"_blank\" href=\"https://community.webroot.com/webroot-business-endpoint-protection-20/disable-execution-of-script-files-303074\">https://community.webroot.com/webroot-business-endpoint-protection-20/disable-execution-of-script-files-303074</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,App,Native Application,Web Application,Software,Firmware,TM-480",
  "libraryId": "1",
  "isHidden": false,
  "guid": "c1a6d43f-93d0-4480-9dd9-624c296ad922",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-10T18:01:02.127",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}