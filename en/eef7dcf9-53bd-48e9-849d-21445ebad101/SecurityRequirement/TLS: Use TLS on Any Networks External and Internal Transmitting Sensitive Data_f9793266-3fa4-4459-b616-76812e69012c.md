{
  "id": "54",
  "name": "TLS: Use TLS on Any Networks External and Internal Transmitting Sensitive Data",
  "description": "<p>All networks, both external and internal, which transmit sensitive data must utilize TLS or an equivalent transport layer security mechanism. It is not sufficient to claim that access to the internal network is &quot;restricted to employees&quot;. Numerous recent data compromises have shown that the internal network can be breached by attackers. In these attacks, sniffers have been installed to access unencrypted sensitive data sent on the internal network.</p><p>SSL, a protocol used to secure network transactions, was developed by Netscape in the mid-90s. Its successor, Transport Layer Security (TLS), was developed by the Internet Engineering Task Force as an enhancement to SSL. The basic operation the two protocols is the same, but TLS incorporates improvements found as SSL became widely used. TLS 1.0 is documented in RFC 2246. TLS 1.1, defined in RFC 4346, corrects some vulnerabilities in the earlier version.SSL and TLS were developed primarily to protect Web transactions, but they can be used to protect any type network traffic that utilizes TCP at the transport layer. Both SSL and TLS are located above TCP in the protocol stack. Applications that interface with TCP when security is not required interface with SSL or TLS when security is required.The position the protocols above TCP means protocol data can traverse a firewall using Network Address Translation (NAT). But an application must be specifically designed for SSL or TLS, since internal logic in the application must determine when to utilize the protocols or when to make calls to TCP directly. All commonly used browsers support both SSL and TLS. SSL VPN vendors provide support for other applications.</p><p><br /></p><p><b>Implementation:</b></p><p>Software acting as an SSL or TLS client requests a connection with a server. The server responds by sending its certificate. The client verifies that it has connected with the desired party by examining the certificate. The certificate contains the server's domain name, the server's public key, the domain name of the issuing CA and the issuing CA's digital signature. The client:Checks that the CA issuing the certificate is on its list of approved CAs.</p><p>If it is, the client uses the CA's public key, included in the approved CA list, along with the CA's digital signature to verify that the certificate has not been altered since it was created by the CA.</p><p>Finally, the client checks that the server's domain name supplied in the certificate matches the domain name of the requested server.</p><p>If authentication of the client is required, the server follows the same steps as those described above.</p><p>Once the identity of the endpoints is verified, data may begin to flow. Symmetric key encryption is employed instead of continuing to use public key encryption to reduce the high computation load required by public key. SSL and TLS also use message authentication codes (MACs) to protect against man-in-the-middle attacks, in which the data is intercepted and modified between the sender and receiver.The development of SSL and TLS relied upon years of careful development of authentication, encryption and MAC techniques, but they have made e-commerce possible. The fact that the protocols are implemented in browsers has also made SSL VPNs easy to use.</p><p><br /></p><p>Reference: <a href=\"https://searchnetworking.techtarget.com/tip/How-SSL-and-TLS-secure-network-transactions\" target=\"_blank\">https://searchnetworking.techtarget.com/tip/How-SSL-and-TLS-secure-network-transactions</a></p>",
  "labels": "",
  "libraryId": "1",
  "isHidden": false,
  "guid": "f9793266-3fa4-4459-b616-76812e69012c",
  "riskId": 1,
  "isCompensatingControl": false,
  "riskName": "Very High",
  "isReadOnlyLibraryEntity": false,
  "lastUpdated": "2021-08-02T14:15:26.393",
  "libraryGuid": "eef7dcf9-53bd-48e9-849d-21445ebad101"
}