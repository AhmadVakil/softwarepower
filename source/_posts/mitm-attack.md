---
title: MitM attack
date: 2016-04-04T17:40:23.432Z
updated: 2016-04-04T17:40:00.000Z
category:
  - Security & Hacking
comments: true
---
A MitM attack occurs when a hacker inserts itself between the communications of a client and a server. Here are some common types of man-in-the-middle attacks:


Session hijacking

In this type of MitM attack, an attacker hijacks a session between a trusted client and network server. The attacking computer substitutes its IP address for the trusted client while the server continues the session, believing it is communicating with the client. For instance, the attack might unfold like this:



A client connects to a server.

The attacker’s computer gains control of the client.

The attacker’s computer disconnects the client from the server.

The attacker’s computer replaces the client’s IP address with its own IP address and

spoofs the client’s sequence numbers.

The attacker’s computer continues dialog with the server and the server believes it is still communicating with the client.

IP Spoofing

IP spoofing is used by an attacker to convince a system that it is communicating with a known, trusted entity and provide the attacker with access to the system. The attacker sends a packet with the IP source address of a known, trusted host instead of its own IP source address to a target host. The target host might accept the packet and act upon it.



Replay

A replay attack occurs when an attacker intercepts and saves old messages and then tries to send them later, impersonating one of the participants. This type can be easily countered with session timestamps or nonce (a random number or a string that changes with time).



Currently, there is no single technology or configuration to prevent all MitM attacks. Generally, encryption and digital certificates provide an effective safeguard against MitM attacks, assuring both the confidentiality and integrity of communications. But a man-in-the-middle attack can be injected into the middle of communications in such a way that encryption will not help — for example, attacker “A”  intercepts public key of person “P” and substitute it with his own public key. Then, anyone wanting to send an encrypted message to P using P’s public key is unknowingly using A’s public key. Therefore, A can read the message intended for P and then send the message to P, encrypted in P’s real public key, and P will never notice that the message was compromised. In addition, A could also modify the message before resending it to P. As you can see, P is using encryption and thinks that his information is protected but it is not, because of the MitM attack.



So, how can you make sure that P’s public key belongs to P and not to A? Certificate authorities and hash functions were created to solve this problem. When person 2 (P2) wants to send a message to P, and P wants to be sure that A will not read or modify the message and that the message actually came from P2, the following method must be used:



P2 creates a symmetric key and encrypts it with P’s public key.

P2 sends the encrypted symmetric key to P.

P2 computes a hash function of the message and digitally signs it.

P2 encrypts his message and the message’s signed hash using the symmetric key and sends the entire thing to P.

P is able to receive the symmetric key from P2 because only he has the private key to decrypt the encryption.

P, and only P, can decrypt the symmetrically encrypted message and signed hash because he has the symmetric key.

He is able to verify that the message has not been altered because he can compute the hash of received message and compare it with digitally signed one.

P is also able to prove to himself that P2 was the sender because only P2 can sign the hash so that it is verified with P2 public key.

Resource: blog.netwrix.com
