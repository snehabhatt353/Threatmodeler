{
  "id": "44",
  "name": "Authentication - Remember Password",
  "description": "Authentication - Remember Password:<br />The \"remember my password\" mechanism can be implemented with one of the following methods:<br /><br />&nbsp; &nbsp; Allowing the \"cache password\" feature in web browsers. Although not directly an application mechanism, this can and should be disabled.<br />&nbsp; &nbsp; Storing the password in a permanent cookie. The password must be hashed/encrypted and not sent in the clear.&nbsp;<br /><br />For the first method, check the HTML code of the login page to see whether browser caching of the passwords is disabled. The code for this will usually be along the following lines:&nbsp;<br /><br />&lt;INPUT TYPE=\"password\" AUTOCOMPLETE=\"off\"&gt;<br /><br />The password autocomplete should always be disabled, especially in sensitive applications, since an attacker, if able to access the browser cache, could easily obtain the password in cleartext (public computers are a very notable example of this attack). To check the second implementation type, examine the cookies stored by the application. Verify that the credentials are not stored in cleartext, but are hashed. Examine the hashing mechanism: if it is a common, well-known algorithm, check for its strength; in homegrown hash functions, attempt several usernames to check whether the hash function is easily guessable. Additionally, verify that the credentials are only sent during the login phase, and not sent together with every request to the application.&nbsp;<br />",
  "labels": "",
  "libraryId": "1",
  "guid": "c6cb2588-30ea-4e23-bb62-67466d5947db",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}