{
  "id": "38",
  "name": "SOAP: Element Duplication",
  "description": "Sometimes we might not be able to hack a Web Service directly, but we can deduce how the Web Service behaves by sending it unexpected XML. One way is sending double elements, like this:\n\n<login>\n  <username> eviware</username>\n  <password> s0ApU1R0ck5</password>\n  <password> s0ApU1R0ck5</password>\n</login>\n\nYou might get a response like this\n\n<loginresponse>\n<error>password is allowed only once and must be at least 6 characters and at most 20 characters.</error>\n</loginresponse>\n\nAlso try that in several permutations:\n\n<login>\n  <username> eviware</username>\n  <username> eviware</username>\n  <password> s0ApU1R0ck5</password>\n  <password> s0ApU1R0ck5</password>\n</login>\n\nOr:\n\n<login>\n  <username> eviware</username>\n  <username> eviware</username>\n  <username> eviware</username>\n  <password> s0ApU1R0ck5</password>\n</login>\n\nDon't stop there! It is just a matter of cloning a TestStep and then changing it to be a new test. ",
  "labels": "",
  "libraryId": "1",
  "guid": "ba0b2f8e-0791-4e64-a3f0-a7d8a783f5e1",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}