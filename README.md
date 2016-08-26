# IdentityManager

The SocIoTal IdM is composed of five main components:

* SocIoTal-IdM-Android-Client: It is an android application that allows obtaining Idemix credentials from the Issuer server. It also allows interact with the Verifier server which can validate the partial identity derived from the credential.

* SocIoTal-Issuer-Server: It is a web application implemented with Java servlets and XML-RPC which allows generating Idemix credentials for clients. Communications are done by https. The client must be authenticated against the Issuer using a valid certificate. The Issuer also support the verification functionality.

* SocIoTal-Verifier-Server: It is a web application, also implemented with Java servlets and XML-RPC, which is able to validate partial identities presented by the client application.

* SocIoTal-IdM-Enabled-Capability Manager: The IdM-Enabled-Capability-Manager is a web application that allows users to obtain capability tokens using their partial identities. In other words, it allows authenticating and demonstrating their attributes by means of Idemix proofs of having a valid credential issued by the Issuer.

* SocIoTal IdM KeyRock Client: The SocIoTal IdM KeyRock Client Java library provides a basic API for identity management by implementing a client to interact with the FIWARE KeyRock server. To carry out such communication, the SCIM 2.0 and Identity API v3 interfaces provided by this IdM are used.
