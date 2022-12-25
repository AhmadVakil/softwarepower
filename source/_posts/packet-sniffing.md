---
title: Packet sniffing
date: 2015-11-17T21:36:13.405Z
updated: 2015-11-17T21:36:00.000Z
category:
  - Security & Hacking
comments: true
---
## **What is Packet Sniffing?**

When any data has to be transmitted over the computer network, it is broken down into smaller units at the sender’s node called data packets and reassembled at receiver’s node in original format. It is the smallest unit of communication over a computer network. It is also called a block, a segment, a datagram or a cell. The act of capturing data packet across the computer network is called packet sniffing. It is similar to as wire tapping to a telephone network. It is mostly used by crackers and hackers to collect information illegally about network. It is also used by ISPs, advertisers and governments.

![](/images/packsniffer.png)


**ISPs use packet sniffing to track all your activities such as:**

\- who is receiver of your email

\- what is content of that email

\- what you download

\- sites you visit

\- what you looked on that website

\- downloads from a site

\- streaming events like video, audio, etc.

**Advertising agencies or internet advertising agencies are paid according to:**


\- number of ads shown by them.

\- number of clicks on their ads also called PPC (pay per click).

To achieve this target, these agencies use packet sniffing to inject advertisements into the flowing packets. Most of the time these ads contain malware.


**Government agencies use packet sniffing to:**

\- ensure security of data over the network.

\- track an organisation’s none encrypted data.

**Packet Sniffer**

Packet sniffing is done by using tools called packet sniffer. It can be either filtered or unfiltered. Filtered is used when only specific data packets have to be captured and Unfiltered is used when all the packets have to be captured. WireShark, SmartSniff are examples of packet sniffing tools.


**How to prevent packet sniffing**

\- Encrypting data you send or receive.

\- using trusted Wi-Fi networks.

\- Scanning your network for dangers or issues.

**What is Wireshark?**

Wireshark is a free and open-source packet analyzer. It is used for network troubleshooting, analysis, software and communications protocol development, and education. Originally named Ethereal, the project was renamed Wireshark in May 2006 due to trademark issues.

Wireshark is cross-platform, using the Qt widget toolkit in current releases to implement its user interface, and using pcap to capture packets; it runs on Linux, macOS, BSD, Solaris, some other Unix-like operating systems, and Microsoft Windows. There is also a terminal-based (non-GUI) version called TShark. Wireshark, and the other programs distributed with it such as TShark, are free software, released under the terms of the GNU General Public License.

In the late 1990s, Gerald Combs, a computer science graduate of the University of Missouri–Kansas City, was working for a small Internet service provider. The commercial protocol analysis products at the time were priced around $1500 and did not run on the company's primary platforms (Solaris and Linux), so Gerald began writing Ethereal and released the first version around 1998. The Ethereal trademark is owned by Network Integration Services.


In May 2006, Combs accepted a job with CACE Technologies. Combs still held copyright on most of Ethereal's source code (and the rest was re-distributable under the GNU GPL), so he used the contents of the Ethereal Subversion repository as the basis for the Wireshark repository. However, he did not own the Ethereal trademark, so he changed the name to Wireshark. In 2010 Riverbed Technology purchased CACE and took over as the primary sponsor of Wireshark. Ethereal development has ceased, and an Ethereal security advisory recommended switching to Wireshark.

Wireshark has won several industry awards over the years, including eWeek, InfoWorld, and PC Magazine. It is also the top-rated packet sniffer in the Insecure.Org network security tools survey and was the SourceForge Project of the Month in August 2010.


Combs continues to maintain the overall code of Wireshark and issue releases of new versions of the software. The product website lists over 600 additional contributing authors.

**Wireshark application**

![](/images/wireshark-captured-data-panes-59512e265f9b58f0fc7b1f17.png)

References: geeksforgeeks, Wikipedia
