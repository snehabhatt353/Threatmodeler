{
  "id": "128",
  "name": "Authentication Bypass- Gray Box Testing",
  "description": "If an attacker has been able to retrieve the application source code by exploiting a previously discovered vulnerability (e.g., directory traversal), or from a web repository (Open Source Applications), it could be possible to perform refined attacks against the implementation of the authentication process.\n\n\nIn the following example (PHPBB 2.0.13 - Authentication Bypass Vulnerability), at line 5 the unserialize() function parses a user supplied cookie and sets values inside the $row array. At line 10 the user's MD5 password hash stored inside the back end database is compared to the one supplied.\n\n1.  if ( isset($HTTP_COOKIE_VARS[$cookiename . '_sid']) ||\n2.  {\n3.  $sessiondata = isset( $HTTP_COOKIE_VARS[$cookiename . '_data'] ) ?\n4. \n5.  unserialize(stripslashes($HTTP_COOKIE_VARS[$cookiename . '_data'])) : array();\n6. \n7.  $sessionmethod = SESSION_METHOD_COOKIE;\n8.  }\n9. \n10. if( md5($password) == $row['user_password'] && $row['user_active'] )\n11. \n12. {\n13. $autologin = ( isset($HTTP_POST_VARS['autologin']) ) ? TRUE : 0;\n14. }\n\nIn PHP, a comparison between a string value and a boolean value (1 - \"TRUE\") is always \"TRUE\", so by supplying the following string (the important part is \"b:1\") to the unserialize() function, it is possible to bypass the authentication control:\n\na:2:{s:11:\"autologinid\";b:1;s:6:\"userid\";s:1:\"2\";}\n\nReference: https://www.owasp.org/index.php/Testing_for_Bypassing_Authentication_Schema_(OTG-AUTHN-004)",
  "labels": "OWASP",
  "libraryId": "1",
  "guid": "f59b215b-e714-4645-9fca-9a8d9b0a2884",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}