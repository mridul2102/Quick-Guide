# TLS and SSL status on Machine
<br>

## can tls and ssl can be simontaniously enabled on a machine ?
Technically, both TLS and SSL can be enabled on a machine, but it's not recommended due to security concerns. Enabling both SSL and TLS on the same server can introduce compatibility issues and potential security vulnerabilities.

When a client (such as a web browser) connects to a server, it negotiates which protocol version to use during the initial handshake. If both SSL and TLS are enabled on the server, the negotiation process may lead to using SSL, which is less secure. This could expose the communication to known vulnerabilities in SSL.

As mentioned earlier, SSL has been deprecated and is considered insecure due to the discovery of various vulnerabilities over the years. The latest TLS versions (TLS 1.2 and TLS 1.3) have addressed these issues and offer stronger security. For this reason, it is strongly recommended to disable SSL and only enable TLS on your server.

Modern web browsers and applications have moved away from supporting SSL and encourage the use of TLS. Most server configurations allow you to specifically enable TLS while disabling SSL, ensuring a more secure and efficient communication channel between clients and servers.