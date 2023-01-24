{
  "id": "92",
  "name": "Brute Force - Determine secret testing procedure",
  "description": "Determine how a potential guess of the secret may be tested. This may be accomplished by comparing some manipulation of the secret to a known value, use of the secret to manipulate some known set of data and determining if the result displays specific characteristics (for example, turning cryptotext into plaintext), or by submitting the secret to some external authority and having the external authority respond as to whether the value was the correct secret. \nIdeally, the attacker will want to determine the correctness of their guess independently since involvement of an external authority is usually slower and can provide an indication to the defender that a brute-force attack is being attempted.\n\nAttack Step Techniques:\n1.   Determine if there is a way to parallelize the attack. Most brute force attacks can take advantage of parallel techniques by dividing the search space among available resources, thus dividing the average time to success by the number of resources available. If there is a single choke point, such as a need to check answers with an external authority, the attackers' position is significantly degraded.\n\nReference: https://capec.mitre.org/data/definitions/112.html",
  "labels": "CAPEC",
  "libraryId": "1",
  "guid": "dc76bd62-35d1-4659-8a1e-b88df81e59a3",
  "isHidden": false,
  "isReadOnlyLibraryEntity": false,
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}