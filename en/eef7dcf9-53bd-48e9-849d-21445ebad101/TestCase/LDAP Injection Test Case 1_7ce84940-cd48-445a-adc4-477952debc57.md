{
  "id": "102",
  "name": "LDAP Injection Test Case 1",
  "description": "LDAP Injection Test Case 1<br />In a page with a user search form the following code is responsible to catch input value and generate a LDAP query that will be used in LDAP database.<br /><br />&nbsp;&lt;input type=\"text\" size=20 name=\"userName\"&gt;Insert the username&lt;/input&gt;&nbsp;<br /><br />The LDAP query is narrowed down for performance and the underlying code for this function might be the following:<br /><br />&nbsp;String ldapSearchQuery = \"(cn=\" + $userName + \")\";<br />&nbsp;System.out.println(ldapSearchQuery);&nbsp;<br /><br />If the variable $userName is not validated, it could be possible accomplish LDAP injection, as follows:<br /><br />&nbsp; &nbsp; If a user puts &ldquo;*&rdquo; on box search, the system may return all the usernames on the LDAP base<br />&nbsp; &nbsp; If a user puts &ldquo;jonys) (| (password = * ) )&rdquo;, it will generate the code bellow revealing jonys&rsquo; password ( cn = jonys ) ( | (password = * ) )<br /><br />Reference:https://www.owasp.org/index.php/LDAP_injectiono<br />",
  "labels": "OWASP",
  "libraryId": "1",
  "guid": "7ce84940-cd48-445a-adc4-477952debc57",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}