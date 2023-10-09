---
description: Local Interconnected Network
---

# LIN

It acts as a supplement to CAN, it has a lower performance but is very cost effective. Some major points of LIN are

* LIN clusters consist of 1 master and up to [16 slave nodes](https://en.wikipedia.org/wiki/Local\_Interconnect\_Network#Overview)
* Single wire (+ground) with 1-20 kbit/s at max 40 m bus length
* Variable data length (2, 4, 8 bytes)
* LIN supports error detection, checksums & configuration
* CAN uses 11 or 29 bit identifiers vs 6 bit identifiers in LIN

<div>

<figure><img src="https://canlogger1000.csselectronics.com/img/LIN-bus-vs-CAN-bus-Local-Interconnect-Network.svg" alt="" width="375"><figcaption><p>LIN interfacing with the CAN</p></figcaption></figure>

 

<figure><img src="https://canlogger1000.csselectronics.com/img/LIN-bus-example-window-control-car-CAN-bus.svg" alt="" width="375"><figcaption><p>Window control example</p></figcaption></figure>

</div>

A master node loops through each of the slave nodes, sending a request for information - and each slave responds with data when polled. The data bytes contain LIN bus signals (in raw form).  The LIN bus message frame consists of a header and a response. Typically, the LIN master transmits a header to the LIN bus. This triggers a slave, which sends up to 8 data bytes in response.&#x20;

<div>

<figure><img src="https://canlogger1000.csselectronics.com/img/LIN-Bus-Frame-Message-Header-Response-Master-Slave.svg" alt="" width="375"><figcaption><p>Data Frame </p></figcaption></figure>

 

<figure><img src="https://canlogger1000.csselectronics.com/img/LIN-Bus-Data-Flow-Transmission-Header-Response.svg" alt="" width="188"><figcaption><p>LIN working</p></figcaption></figure>

</div>

* Break - Start of Frame
* Sync -  A default value to calculate the timing between edges
* ID  -  for slaves to respond to the particular ID's and whether to transmit/receive/ignore and also determine the validity of the ID field (based on the parity bits)

Ref :  [https://www.csselectronics.com/pages/lin-bus-protocol-intro-basics](https://www.csselectronics.com/pages/lin-bus-protocol-intro-basics)

\


\
