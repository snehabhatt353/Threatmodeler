{
  "id": "42",
  "name": "Key Management: Use independent keys when multiple keys are required",
  "description": "<p>To improve the strength of the encryption it is always good to have independent keys instead of same keys multiple times.</p><p>For example In each Triple DES encryption, a block of 64 bits of data is encrypted three times with same or different keys.</p><p>In each case the middle operation is the reverse of the first and last. This improves the strength of the algorithm when using a set of independent keys instead of the same key.</p><p>Ensure that key material is independent. That is, do not choose a second key which is easily related to the first (or any preceding) keys.</p><p><br /></p><p>Reference:</p><p><a href=\"https://sg.inflibnet.ac.in/bitstream/10603/27521/11/11_chapter%203.pdf\" target=\"_blank\">https://sg.inflibnet.ac.in/bitstream/10603/27521/11/11_chapter%203.pdf</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Key Management Server,TM-277",
  "libraryId": "1",
  "isHidden": false,
  "guid": "6df71424-ebf5-426b-be24-6fbf1bf21ad9",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-09-29T15:34:56.507",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}