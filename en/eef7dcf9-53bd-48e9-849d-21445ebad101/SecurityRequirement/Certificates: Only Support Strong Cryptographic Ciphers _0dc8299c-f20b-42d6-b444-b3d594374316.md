{
  "id": "64",
  "name": "Certificates: Only Support Strong Cryptographic Ciphers ",
  "description": "<p>Each protocol (SSLv3, TLSv1.0, etc) provides cipher suites. As of TLS 1.2, there is support for over 300 suites (320+ and counting), including national vanity cipher suites. </p><p>The strength of the encryption used within a TLS session is determined by the encryption cipher negotiated between the server and the browser. </p><p>In order to ensure that only strong cryptographic ciphers are selected the server must be modified to disable the use of weak ciphers. It is recommended to configure the server to only support strong ciphers and to use sufficiently large key sizes. </p><p><b>In general, the following should be observed when selecting CipherSuites:</b></p><ul><li>Disable cipher suites that do not offer authentication (NULL ciphersuites, aNULL or eNULL)\n</li><li>Disable anonymous Diffie-Hellman key exchange (ADH)\n</li><li>Disable export level ciphers (EXP, eg. ciphers containing DES)\n</li><li>Disable key sizes smaller than 128 bits for encrypting payload traffic\n</li><li>Disable the use of MD5 as a hashing mechanism for payload traffic\n</li><li>Use AES, 3-key 3DES for encryption operated in CBC mode\n    Stream Ciphers which XOR the key stream with plaintext (such as AES/CTR mode)\n</li><li>Use SHA1 or above for digests, prefer SHA2 (or equivalent)\n    Support ephemeral Diffie-Hellman key exchange \n</li></ul>",
  "labels": "ThreatModeler,AppSec and InfraSec,Certificate Authorities,TM-37",
  "libraryId": "1",
  "isHidden": false,
  "guid": "0dc8299c-f20b-42d6-b444-b3d594374316",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2020-09-22T13:26:48.247",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}