{
  "id": "121",
  "name": "Cache Poisoning",
  "description": "We have found a web page, which gets its service name from the \"page\" argument and then redirects (302) to this service.\n\ne.g. http://testsite.com/redir.php?page=http://other.testsite.com/\n\nAnd exemplary code of the redir.php:\n\nrezos@dojo ~/public_html $ cat redir.php\n<?php\nheader (\"Location: \" . $_GET['page']);\n?>\n\n\nHTTP header fields \"Pragma: no-cache\" or \"Cache-Control: no-cache\" will remove the page from cache (if the page is stored in cache, obviously).\n\n\nReference: https://www.owasp.org/index.php/Cache_Poisoning",
  "labels": "OWASP",
  "libraryId": "1",
  "guid": "dfcb1be3-f927-4ec5-aec2-7ea69cbb0210",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}