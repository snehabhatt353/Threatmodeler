{
  "id": "128",
  "name": "Public keys over secure channel",
  "description": "<p>In the SSH public key authentication use case, it is rather typical that the users create (i.e. provision) the key pair for themselves. SSH implementations include easily usable utilities for this (for more information see ssh-keygen and ssh-copy-id).</p><p>Each SSH key pair includes two keys:</p><p>A public key that is copied to the SSH server(s). Anyone with a copy of the public key can encrypt data which can then only be read by the person who holds the corresponding private key. Once an SSH server receives a public key from a user and considers the key trustworthy, the server marks the key as authorized in its authorized_keys file. Such keys are called authorized keys.<br /></p><p>A private key that remains (only) with the user. The possession of this key is proof of the user's identity. Only a user in possession of a private key that corresponds to the public key at the server will be able to authenticate successfully. The private keys need to be stored and handled carefully, and no copies of the private key should be distributed. The private keys used for user authentication are called identity keys.<br /></p><p>Always exchange public keys using a secure channel.</p><p><b>The following simple steps are required to set up public key authentication (for SSH):</b></p><ul><li>Key pair is created (typically by the user). This is typically done with ssh-keygen.</li><li>Private key stays with the user (and only there), while the public key is sent to the server. Typically with the ssh-copy-id utility.</li><li>Server stores the public key (and &quot;marks&quot; it as authorized).</li><li>Server will now allow access to anyone who can prove they have the corresponding private key.</li></ul><p><br /></p><p><b>Reference:</b></p><p><a href=\"https://www.ssh.com/ssh/public-key-authentication\" target=\"_blank\">https://www.ssh.com/ssh/public-key-authentication</a></p>",
  "labels": "ThreatModeler,AppSec and InfraSec,TLS,SSL,TM-81",
  "libraryId": "1",
  "isHidden": false,
  "guid": "1f34318c-cf72-4e18-abca-af34f74fbebf",
  "riskId": 2,
  "isCompensatingControl": false,
  "riskName": "High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-09-29T15:34:56.617",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}