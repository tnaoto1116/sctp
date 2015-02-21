###Stream Control Transmission Protocol
----------

Stream Control Transmission Protocol (SCTP) is a transport-layer protocol 
that can be used on top of IP networks for end-to-end communications. 
SCTP has been standardized by the IETF in a series of RFCs that define the protocol, 
its applicability to other protocols, and its management. 
SCTP was originally defined in RFC 2960 in October 2000, 
but was then updated with RFC 4960 in September 2007.

SCTP is similar to TCP in many ways. They are both unicast 
connection-oriented protocols that provide reliable transport, 
in-sequence packet delivery and rate-adaptive congestion control.
TCP has an additive 16-bit checksum (RFC 1071) 
and SCTP has a 32-bit CRC (RFC 4960).

SCTP may be more resistant to Man-In-The-Middle (MITM) 
and Denial of Service (DoS) attacks. SCTP uses a cookie 
mechanism in the initial connection procedure (INIT ACK). 
SCTP doesn't allow for half-open connections so it is 
more resilient to flooding, masquerade attacks.

SCTP also has many features that are similar to UDP. 
Both support unreliable transport and out-of-order packet 
delivery. SCTP does have a 12-byte header compared to 
UDP's 8-byte header, but that is negligible when 
comparing performance between the protocols.

SCTP is able to do some things that UDP can't achieve. 
SCTP is able to deal with Path MTU Discovery (PMTUD) 
and fragmentation. SCTP has connection detection and 
SCTP can detect dropped and duplicated packets. Therefore, 
not every application is well suited to either TCP or UDP 
and SCTP can provide the best of both TCP and UDP capabilities.

###MANIFEST
--------
```
.
|-- bin
|-- doc
    |--LICENCE.txt
    |--COPYING.txt
    |--ROADMAP.txt
    |--INSTALL.txt
    |--ChangeLog.txt
    `--material
|-- src
    |-- apps
    |-- func_tests
    |-- include
    |   `-- netinet
    |-- lib
    |-- testlib
    `-- withsctp
```
You may want to check the following files:
```
LICENCE	  Licensing terms of this repository

COPYING	  Licensing terms of other pieces of the package

ROADMAP		A tour around the files

INSTALL   How to install and run.

ChangeLog	What has changed since the last release?
```



###GOALS
- [ ]



###FEATURES
-----------



###WEB SITES AND CONTACT INFO
---------------------------
You can find us on freenode network in channel #openSCTP
