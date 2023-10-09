# Ethernet

The Ethernet protocol is a wired network that allows computers to communicate with each other. The Ethernet protocol uses a star topology or linear bus

Ethernet architecture is based on the concept of connecting multiple computers to a long cable, called the ether, to form a bus structure. Each computer has an Ethernet adapter with a unique 48-bit address. The adapters are programmed with globally unique MAC addresses to specify the source and destination of each data packet.

<figure><img src="https://www.elprocus.com/wp-content/uploads/Ethernet-Protocol-Architecture.jpg" alt=""><figcaption><p>Ethernet Architecture</p></figcaption></figure>

The data link layer in the network system mainly addresses the way that data packets are transmitted from one type of node to another. Ethernet uses an access method called CSMA/CD (Carrier Sense Multiple Access/Collision Detection).

The Logical Link Control (LLC) handles the communication between the upper layers & the lower layers. The LLC layer uses the data of [network protocol](https://www.elprocus.com/network-protocol-types-and-layers/) like IPv4 packet & adds control data to help in delivering the packet toward the destination node. The second layer (Layer 2) interacts through the higher layers using LLC which can be implemented within software & its implementation is independent of the physical devices.

Ethernet Frame Overview

<figure><img src="https://www.freecodecamp.org/news/content/images/2022/10/image-98.png" alt=""><figcaption><p>Ethernet Frame</p></figcaption></figure>

* Preamble - A sequence of 10101011 in order to synchronize the bits and last bit is the start bit
* Destination Address - If the device the address is matched with destination address then the device allows transmission
* Source Address - It contains the address of the source
* Length -  This field size is 2-byte long that specifies the entire Ethernet frame length
* Data Field - Contains the data
* CRC Field - It is the last pattern with 4 Bytes. This field includes 32-bits of data hash code.
