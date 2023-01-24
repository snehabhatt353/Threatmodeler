{
  "id": "23",
  "name": "Reflected Cross Site Scripting - HTTP Parameter Pollution  ",
  "description": "Reflected Cross Site Scripting - HTTP Parameter Pollution (HPP) :<br /><br />Another method to bypass filters is the HTTP Parameter Pollution, this technique was first presented by Stefano di Paola and Luca Carettoni in 2009 at the OWASP Poland conference. See the Testing for HTTP Parameter pollution for more information. This evasion technique consists of splitting an attack vector between multiple parameters that have the same name. The manipulation of the value of each parameter depends on how each web technology is parsing these parameters, so this type of evasion is not always possible. If the tested environment concatenates the values of all parameters with the same name, then an attacker could use this technique in order to bypass pattern- based security mechanisms.<br />Regular attack:<br /><br />http://example/page.php?param=&lt;script&gt;[...]&lt;/script&gt;<br /><br />Attack using HPP:<br /><br />http://example/page.php?param=&lt;script&amp;param=&gt;[...]&lt;/&amp;param=script&gt;",
  "labels": "",
  "libraryId": "1",
  "guid": "b9696b94-84c1-49e5-891e-11aba80a10dc",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}