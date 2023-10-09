---
description: Brief on flexray
---

# Flexray

The FlexRay protocol is a high-speed, fault-tolerant communication system for automotive electronics. It supports star, line and hybrid topologies. FlexRay supports single- and dual-channel configurations which consist of one or two pairs of wires respectively. Differential signaling on each pair of wires reduces the effects of external noise on the network without expensive shielding. Some pointers of flexray are

* Time triggered protocol - that allows data transfer within a time interval (in micro-seconds) as well as CAN-like dynamic event-driven data to handle a large variety of frames
* It has a separate space for static and dynamic data&#x20;
* While CAN needs only the configuration of baud rate, flexray requires the knowledge of the network configuration
* At one time only one node can write data to BUS.



FlexRay manages multiple nodes with a Time Division Multiple Access or TDMA scheme. Every FlexRay node is synchronized to the same clock, and each nodes waits for its turn to write on the bus

<figure><img src="https://ni.scene7.com/is/image/ni/FlexRay_Cycle_Overview?scl=1" alt=""><figcaption><p>Flexray</p></figcaption></figure>

Flexray communication cycle

* Static segment- reserved slot for deterministic data, it is the space in the cycle dedicated to scheduling a number of time-triggered frames
* Dynamic segment- behaves as CAN
* Symbol window - used for signaling and maintenance
* Network Idle Time  - Maintain synchronization between the clocks

Macro tick - smallest practical unit of time

<figure><img src="https://ni.scene7.com/is/image/ni/FlexRay_Single_Cycle?scl=1" alt="" width="375"><figcaption><p>Macrotick</p></figcaption></figure>

FlexRay controllers actively synchronize themselves and adjust their local clocks so that the macrotick occurs at the same point in time on every node across the network.

The Data Frame of flexray

<figure><img src="https://ni.scene7.com/is/image/ni/FlexRay_Frame_Breakdown?scl=1" alt=""><figcaption><p>Data Frame</p></figcaption></figure>

Header format includes, Frame ID, which defines the slot in which the frame should be transmitted and is used for prioritizing event-triggered frames, The Payload Length, contains the number of words which are transferred in the frame. The Header CRC is used to detect errors.

<figure><img src="https://ni.scene7.com/is/image/ni/FlexRay_Frame_Bits?scl=1" alt=""><figcaption><p>Header part</p></figcaption></figure>

Payload contains the actual data&#x20;

<figure><img src="https://ni.scene7.com/is/image/ni/FlexRay_Payload?scl=1" alt=""><figcaption><p>Payload</p></figcaption></figure>

Trailer contain 8 bit CRC's to detect errors

<figure><img src="https://ni.scene7.com/is/image/ni/FlexRay_Trailer?scl=1" alt=""><figcaption><p>Trailer</p></figcaption></figure>

Flexray can transmit upto 10Mbit/s.&#x20;

Ref : [https://www.ni.com/en/shop/seamlessly-connect-to-third-party-devices-and-supervisory-system/flexray-automotive-communication-bus-overview.html#:\~:text=Back%20to%20top-,The%20FlexRay%20Protocol,a%20large%20variety%20of%20frames.](https://www.ni.com/en/shop/seamlessly-connect-to-third-party-devices-and-supervisory-system/flexray-automotive-communication-bus-overview.html)
