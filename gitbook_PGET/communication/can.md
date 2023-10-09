---
description: Controller Area Network
---

# CAN

A CAN network consists of a number of CAN nodes which are linked via a physical transmission medium. In practice, the CAN network is usually based on a line topology with a linear bus to which a number of electronic control units are each connected via a CAN interface.

<div align="left">

<figure><img src="https://canlogger1000.csselectronics.com/img/CAN-bus-intro-tutorial-controller-area-network.svg" alt="" width="375"><figcaption><p>CAN network</p></figcaption></figure>

 

<figure><img src="https://www.csselectronics.com/cdn/shop/files/twisted-can-bus-wiring-harness-high-low-green-yellow.svg?v=1633690039" alt="" width="188"><figcaption><p>CAN lines</p></figcaption></figure>

</div>

CAN bus consists of two wires, CAN low and CAN high and each ECU has the ability to receive and transmit the data to the BUS. A CAN network can have multiple masters

The maximum data rate is 1 Mbit/s. A maximum network extension of about 40 meters is allowed.&#x20;

<figure><img src="https://canlogger1000.csselectronics.com/img/CAN-bus-ECU-node-communication-send-accept-reject.svg" alt=""><figcaption><p>Working Of CAN</p></figcaption></figure>

An ECU can prepare and broadcast information (e.g. sensor data) via the CAN bus (consisting of two wires, CAN low and CAN high). The broadcasted data is accepted by all other ECUs on the CAN network - and each ECU can then check the data and decide whether to receive or ignore it.

<div>

<figure><img src="../.gitbook/assets/download.png" alt="" width="375"><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/download (1).png" alt="" width="320"><figcaption></figcaption></figure>

</div>

Each ECU requires a CAN interface which consists of CAN controller and CAN transceiver. The [CAN transceiver](https://elearning.vector.com/mod/page/view.php?id=339) connects the CAN controller to the physical transmission medium. Twisting of the two lines reduces the magnetic field considerably. Therefore, in practice [twisted pair](https://elearning.vector.com/mod/page/view.php?id=355) conductors are generally used as the physical transmission medium

<figure><img src="../.gitbook/assets/download (2).png" alt="" width="315"><figcaption></figcaption></figure>

A [data frame](https://elearning.vector.com/mod/page/view.php?id=345) can transport a maximum payload of eight bytes. For that there is the so-called data field, which is framed by many other fields that are required to execute the CAN communication protocol. They include the message address (identifier or ID), data length code (DLC), checksum (cyclic redundancy check sequence — CRC sequence) and RX acknowledgement located in the acknowledgement field.

<figure><img src="../.gitbook/assets/download (3).png" alt=""><figcaption><p>DATA Frame</p></figcaption></figure>

* SOF - Start of Frame bit
* ID & RTR - sets the priority and also acceptance/receiver filtering
* IDE - Identifier extension bit to differentiate between standard format and extended format
* DLC - Data Length Code - number of payload bits
* CRC & ACK - Checksum and acknowledgement
* EOF -  After this the transmission of a data frame is terminated by seven recessive bits

Besides the data frame used to transport data, there is the remote frame — a frame type used to request data, i.e. data frames, from any CAN node.

<div>

<figure><img src="https://canlogger1000.csselectronics.com/img/CAN-bus-frame-standard-message-SOF-ID-RTR-Control-Data-CRC-ACK-EOF.svg" alt="" width="375"><figcaption><p>CAN Frame</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/download (5).png" alt="" width="375"><figcaption><p>Physical signal</p></figcaption></figure>

</div>

High-speed and low-speed CAN are types of Controller Area Network (CAN). CAN is a serial bus system that connects sensors and controllers in a vehicle. High-speed CAN has a data rate of up to 1 Mbit/s, while low-speed CAN has a data rate of up to 125 kbit/s

Ref: [https://www.csselectronics.com/pages/can-bus-simple-intro-tutorial](https://www.csselectronics.com/pages/can-bus-simple-intro-tutorial)
