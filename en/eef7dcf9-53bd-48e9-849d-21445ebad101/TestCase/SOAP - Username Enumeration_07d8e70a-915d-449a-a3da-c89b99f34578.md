{
  "id": "47",
  "name": "SOAP - Username Enumeration",
  "description": "Let's start by iterating; We're looking for any information that might learn us more about system behavior, set up, or data. Anything that helps us getting closer to getting into the target system is what we want. What we're looking for her is even more common than previous scenarios, and this is worrying, because in this case ther target gives up very useful information.\n\nThis is what we do, enter what you know is a non-existing user name: Say that you have a user name and password combination like this:\n\n    User: eviware\n    Password: s0ApU1R0ck5\n\nUse a login like this:\n\n<login>\n  <username> emery bear</username>\n  <password> s0ApU1R0ck5</password>\n</login>\n\nAnd look for a response with the following meaning:\n\n<loginresponse>\n  <error>That user does not exist</error>\n</loginresponse>\n\nThis will allow you to work through a number of user names until find you one that is working.\n\n\n[Source] soapui.org",
  "labels": "",
  "libraryId": "1",
  "guid": "07d8e70a-915d-449a-a3da-c89b99f34578",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}