{
  "id": "107",
  "name": "Host Specific Token",
  "description": "<p>Token based authentication is stateless. We are not storing any information about our user on the server or in a session.<br /></p><p>This takes care of many of the problems with having to store information on the server.<br /></p><p>No session information means your application can scale and add more machines as necessary without worrying about where a user is logged in.<br /><br />Although this implementation can vary, the gist of it is as follows:<br /></p><ol><li>User Requests Access with Username / Password</li><li>Application validates credentials</li><li>Application provides a signed token to the client</li><li>Client stores that token and sends it along with every request</li><li> Server verifies token and responds with data</li></ol><p>Every single request will require the token. This token should be sent in the HTTP header so that we keep with the idea of stateless HTTP requests.<br /></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Exit,TM-193,DemoComp,Registration",
  "libraryId": "1",
  "isHidden": false,
  "guid": "4e5c3cd2-afde-4b4a-8ba4-b092df6dcbb3",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-12-17T15:25:17.533",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}