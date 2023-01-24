{
  "id": "49",
  "name": "SOAP - XPath Injection",
  "description": "XPath injection then basically is like SQL injection in XML documents. Now, user data, for example, is seldom stored in XML Documents, so you might believe you are safe, but often the system you're testing is communicating with another system over Web Services. And what do we use to communicate, what do we send back and forth? XML documents...\n\nNow, when we know why, let's look at how.\n\n<login>\n  string(//user[username/text()='' or '1' = '1' and password/text()='' or '1' = '1'])\n</login>\n\nWe know that from the SQL Injection example, we're trying to let the system log us in. It might not work, but it is very interesting to see how the error has been handled.\n\n \n\nWe can also try to tease the XPath processor in the target system;\n\n<login>\n  string(//user[user_name/text()='' or '1' = '1' and password/text()='' or '1' = '1'])\n</login>\n\nWhat happens when the XPath processor gets a faulty node? Will we get an error message directly from Xalan, Saxon, Microsoft's XPathNavigator?\n\n \n\nYou should of course play around with the XPath expressions some more and try to coax out as much information as possible about the target system.",
  "labels": "",
  "libraryId": "1",
  "guid": "dec0d44d-1bd6-4d6f-b56d-923f2ca31c9a",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}