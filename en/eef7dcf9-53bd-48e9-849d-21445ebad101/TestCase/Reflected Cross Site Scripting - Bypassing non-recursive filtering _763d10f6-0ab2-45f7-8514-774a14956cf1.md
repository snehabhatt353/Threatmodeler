{
  "id": "21",
  "name": "Reflected Cross Site Scripting - Bypassing non-recursive filtering ",
  "description": "Reflected Cross Site Scripting - Bypassing non-recursive filtering :<br />Sometimes the sanitization is applied only once and it is not being performed recursively. In this case the attacker can beat the filter by sending a string like this one:<br /><br />&lt;scr&lt;script&gt;ipt&gt;alert(document.cookie)&lt;/script&gt;<br />",
  "labels": "",
  "libraryId": "1",
  "guid": "763d10f6-0ab2-45f7-8514-774a14956cf1",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}