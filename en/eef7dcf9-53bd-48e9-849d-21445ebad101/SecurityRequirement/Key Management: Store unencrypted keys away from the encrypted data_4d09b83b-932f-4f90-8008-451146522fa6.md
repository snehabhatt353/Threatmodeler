{
  "id": "41",
  "name": "Key Management: Store unencrypted keys away from the encrypted data",
  "description": "<p>The unencrypted keys need to be stored away from the encrypted data if suppose the unencrypted data is stolen along with the keys. It might lead to whole compromise of the system important data which is being encrypted. Malicious users might decrypt the data by using some of the special cryptograhic algorithms.</p><p><b>The following tips can help your organization protect its encryption keys to prevent them falling into the wrong hands or getting lost: <br /></b></p><p>\rPhysically secure encryption systems: The machines and systems that run encryption programs and store the encryption keys should be physically secured with locked doors and other appropriate measures. Access ought be granted to those with adequate knowledge and integrity. </p><p>\rDo not store encryption keys with the data they decrypt: Encryption keys should be stored on separate machines from the data they are used to unlock. When they are both located on the same machine, if that machine is compromised so also are the keys. </p><p>Have an audit trail: Audit logs show who has accessed what data and when. This information can prevent keys from becoming compromised and provide crucial information about the compromise if there is a data breach. <br /></p><p>\rMaintain a secure and frequently updated off-site backup of encryption keys: Having all your encryption keys locked up and on one secure machine does no good if that machine fails. If all the keys are lost in a drive failure, the encrypted data will become inaccessible. </p><p>\rManage encryption key life-cycle: The most secure encryption keys are set to expire after a predetermined time period. No matter how well secured these encryption keys are, if they expire without a new key being issued, saved, backed up, and secured, the keys will be useless. </p><p>Encrypt keys as another layer of security: Encryption works great for securing your data. Why not use it to secure your keys? <br /></p><p>Require multi-factor authentication for any master keys: An authorized staff member should be able to access keys to rebuild databases from encrypted backups in case of a disaster. However, these keys should have the extra layer of security that only multi-factor authentication can offer. <br /></p><p>Make it possible to change keys periodically: Changing keys in the case of a data breach is a necessary precaution. The ability to change keys periodically can also prevent unauthorized access if keys were unknowingly accessed. <br /></p><p>Have a key recovery procedure: Accidental data loss is nearly an inevitable occurrence in computing. Keys will be compromised. Making sure there is a secure procedure for recovering lost keys will guarantee that data will be accessible. <br /></p><p>Keep recovery keys in escrow: In addition to or as an alternative to off-site backup of encryption keys, a trusted third-party could be entrusted with a sealed escrow packet of keys.</p><p>Resource:</p><p><a href=\"https://aspg.com/2013/04/17/10-tips-for-securing-encryption-keys/#.XxCXuyhKg2w\" target=\"_blank\">https://aspg.com/2013/04/17/10-tips-for-securing-encryption-keys/#.XxCXuyhKg2w</a></p><p><br /></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,Key Management Server,TM-189",
  "libraryId": "1",
  "isHidden": false,
  "guid": "4d09b83b-932f-4f90-8008-451146522fa6",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-09-29T15:34:56.493",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}