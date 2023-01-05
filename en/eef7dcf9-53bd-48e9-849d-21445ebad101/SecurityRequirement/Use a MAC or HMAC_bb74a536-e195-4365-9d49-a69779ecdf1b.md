{
  "id": "123",
  "name": "Use a MAC or HMAC",
  "description": "Use a MAC or HMAC. The Message Authentication Code Triple Data Encryption Standard (MACTripleDES) algorithm computes a MAC, and HMACSHA1 computes an HMAC. Both use a key to produce a checksum. With these algorithms, an attacker needs to know the key to generate a checksum that would compute correctly at the receiver.\r\nThe use of HMAC to hash the response from the server can also be used to thwart reflection. The server responds by returning its own challenge as well as hashing the client's challenge, its own challenge and the pre-shared secret. Requiring the client to respond with the HMAC of the two challenges ensures that only the possessor of a valid pre-shared secret can successfully hash in the two values.\r\n",
  "labels": "",
  "libraryId": "1",
  "isHidden": false,
  "guid": "bb74a536-e195-4365-9d49-a69779ecdf1b",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-09-29T15:34:56.587",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}