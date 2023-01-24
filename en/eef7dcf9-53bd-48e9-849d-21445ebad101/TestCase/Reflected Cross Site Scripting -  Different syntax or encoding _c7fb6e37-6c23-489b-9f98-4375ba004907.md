{
  "id": "20",
  "name": "Reflected Cross Site Scripting -  Different syntax or encoding ",
  "description": "<p>Reflected Cross Site Scripting -&nbsp; Different syntax or encoding&nbsp;</p><p>In some cases it is possible that signature-based filters can be simply defeated by obfuscating the attack. Typically you can do this through the insertion of unexpected variations in the syntax or in the econding. These variations are tolerated by browsers when the code is returned, and they could also be accepted by the filter. Following some examples:<br /><br />\"&gt;&lt;script &gt;alert(document.cookie)&lt;/script &gt;<br /><br />\"&gt;&lt;ScRiPt&gt;alert(document.cookie)&lt;/ScRiPt&gt;<br /><br />\"%3cscript%3ealert(document.cookie)%3c/script%3e</p>",
  "labels": "",
  "libraryId": "1",
  "guid": "c7fb6e37-6c23-489b-9f98-4375ba004907",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}