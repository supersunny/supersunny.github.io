---
name: SSH Protocol Implementation
tools: [OpenSSL, Computer Security, C]
image: https://www.thesslstore.com/blog/wp-content/uploads/2018/11/man-in-the-middle-attack.png
description: The SSH protocol is a method for secure remote communication between two nodes on a network. I implemented SSH protocol virtually using OpenSSL library in C language
---

## Objective

The SSH protocol is a method for secure remote communication between two nodes on a network. It contains strong authentication procedure, and it protects the communications security and integrity with strong encryption. It is a secure alternative to the non-protected login protocols and insecure file transfer methods (such as FTP).

![Preview](https://www.thesslstore.com/blog/wp-content/uploads/2018/11/man-in-the-middle-attack.png)

## Implementation
In the situation of communication between a server and a client, Both side need a encrypted message or key to communicate each other. By following the protocol below, Both party can have a secure communication.

(1) A client requests a communication to the server \\
(2) The server sends its public key to the client \\
(3) The client creates a session key and send it encrypted with the server's public key \\
(4) The server decrypts the session key with its private key \\
(5) The server sends a message to confirm that it received the session key \\
(6) The client decrpyts the message from the server by the session key \\
(7) Now, the server and the client can communicate securely with the shared session key \\

For more information, check the link below
<p class="text-center">
{% include elements/button.html link="https://www.dropbox.com/s/bt0a225fozmkivb/SSH_protocol.pdf?dl=0" text="Learn More" %}
</p>