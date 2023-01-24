{
  "id": "48",
  "name": "SOAP - Account Lockout",
  "description": "This security flaw is extra common in Web Services and one that if handled correctly offers very good protection. Web Services aren't as public as web pages and basic security measurements aren't implemented, we probably think that ?Well, the Web Service won't be public so it's a good bet we're not going to be noticed\".\n\nA short unscientific study showed that there are two more reasons why; with web services, we let the prototype go live without actually industrializing it, or the web service is created by rightclicking a method or class in your favorite IDE and chossing \"Publish as Web Service\".\n\nWhat we do to test it is, basically make an loop with a login request that automatically updates the faulty password. If you haven't been locked out after a certain number of tries (how many depends on business requirements, but three should be a good target), you have a potential security risk.\nFirst Request\n\n<login>\n  <username> eviware</username>\n  <password>yesitdoes!1</password>\n</login>\n\nSecond Request\n\n<login>\n  <username> eviware</username>\n  <password>yesitdoes!2</password>\n</login>\n\nAnd so on...\n\nSo what lockout do we choose? Well the usual is after three failed attempts we get locked out for a certain time, like 6-24 hours. One that is very interesting is the Geometrically Increased penalty; for each try you lockout time doubles; the first failed attempt gives you a 1 second delay, the second, 2, the third 4 and so on. This makes the penalty for an honest mistake very slight, and not very deterring you might think, but look at what happens later; after 25 failed attempts the lock out time is 225 seconds or as it is more commonly know; more than a year!. This makes robots or scripts unusable!",
  "labels": "",
  "libraryId": "1",
  "guid": "964f51f0-df8c-4eb5-a560-e07ad8b35a7a",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}