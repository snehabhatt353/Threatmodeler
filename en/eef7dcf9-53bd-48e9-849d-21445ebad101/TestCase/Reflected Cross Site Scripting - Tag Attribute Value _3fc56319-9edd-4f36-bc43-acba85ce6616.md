{
  "id": "19",
  "name": "Reflected Cross Site Scripting - Tag Attribute Value ",
  "description": "Reflected Cross Site Scripting - Tag Attribute Value :<br />Since these filters are based on a blacklist, they could not block every type of expressions. In fact, there are cases in which an XSS exploit can be carried out without the use of &lt;script&gt; tags and even without the use of characters such as \" &lt; &gt; and / that are commonly filtered. For example, the web application could use the user input value to fill an attribute, as shown in the following code:&nbsp;<br /><br />&lt;input type=\"text\" name=\"state\" value=\"INPUT_FROM_USER\"&gt;<br /><br /><br />Then an attacker could submit the following code:&nbsp;<br /><br />\" onfocus=\"alert(document.cookie)<br />",
  "labels": "",
  "libraryId": "1",
  "guid": "3fc56319-9edd-4f36-bc43-acba85ce6616",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}