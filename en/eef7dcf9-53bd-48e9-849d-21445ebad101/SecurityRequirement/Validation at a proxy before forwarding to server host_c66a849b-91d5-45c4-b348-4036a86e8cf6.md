{
  "id": "102",
  "name": "Validation at a proxy before forwarding to server host",
  "description": "<p>The Proxy object is used to define custom behavior for fundamental operations (e.g. property lookup, assignment, enumeration, function invocation, etc).</p><p>In other words, you can make stuff happen when an interaction with an object occurs. This is possible thanks to traps, but we’ll talk more about this in a sec.</p><p>To create a new Proxy you must provide a target and a handler. The target — as MDN states — can be any sort of object (i.e. object, array, function, or proxy). This is the one that will suffer the final side effects (if any) of the interaction with the proxy.</p><p>The handler is another object that defines traps. Traps are functions, set to act when an operation is performed on a proxy. Depending on the operation one trap or another is called. I like to think of traps as some sort of lifecycle hooks. If you’ve worked with a frontend framework (i.e. React), this will be nothing new. For all others — really? — a lifecycle hook is a callback that’s called in a certain point on the lifecycle.</p><p>Of course, proxy traps. So for example, if you want to execute some code when a component is mounted, you’d need to implement the componentDidMount hook right? right? Well, with proxies you can do (almost) the same thing!</p><p>Proxy communication to host, so that communications are terminated at the  proxy, sanitizing the requests before forwarding to server host.</p><p><br /></p><p><b>Reference:</b></p><p><a href=\"https://medium.com/hackernoon/how-i-made-a-validation-library-using-es6-proxy-59df82c1a4c0\" target=\"_blank\">https://medium.com/hackernoon/how-i-made-a-validation-library-using-es6-proxy-59df82c1a4c0</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Proxy Server,Gateway,Router,TM-488",
  "libraryId": "1",
  "isHidden": false,
  "guid": "c66a849b-91d5-45c4-b348-4036a86e8cf6",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-16T19:30:28.937",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}