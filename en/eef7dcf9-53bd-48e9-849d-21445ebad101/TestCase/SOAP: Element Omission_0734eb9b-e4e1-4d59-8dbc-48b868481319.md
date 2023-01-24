{
  "id": "39",
  "name": "SOAP: Element Omission",
  "description": "Element Omission is quite similar to Element Duplication, but the opposite. Instead of having extra elements, we enter less elements in the request:\n\n<login>\n  <username> eviware</username>\n</login>\n\nTo your surprise, you might be getting:\n\n<loginresponse>\n  <errror>element password is expected.</error>\n</loginresponse>\n\nYou should do clone and change here as well, we'll try the orther way around:\n\n<login>\n  <password>s0ApU1R0ck5</password>\n</login>\n\nand without any elements at all:\n\n<login>\n</login>",
  "labels": "",
  "libraryId": "1",
  "guid": "0734eb9b-e4e1-4d59-8dbc-48b868481319",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}