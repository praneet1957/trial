---
description: Hardware in Loop simulation
---

# HiL

In Hardware in Loop simulation, we test the real controller with a real time virtual environment which is simulated on a PC and is the plant of our system.&#x20;

Why HiL?

<figure><img src="https://www.mathworks.com/help/simscape/ug/rt_mbd_design_to_realization_flow_chart.png" alt=""><figcaption><p>Model Based Design</p></figcaption></figure>

Above we can see at what stage of the design process does the Hardware-in-Loop simulation fits into.

<figure><img src="https://www.mathworks.com/help/simscape/ug/rt_hil_definition.png" alt=""><figcaption><p>Hardware in Loop  Simulation</p></figcaption></figure>

* An HIL test system consists of three primary components: a real-time processor, I/O interfaces, and an operator interface. The real-time processor is the core of the HIL test system.
* A dedicated real-time processor executes mathematical models which emulate engine dynamics
* In addition, an [I/O](https://en.wikipedia.org/wiki/I/O) unit allows the connection of vehicle [sensors](https://en.wikipedia.org/wiki/Sensors) and [actuators](https://en.wikipedia.org/wiki/Actuators) (which usually present high degree of non-linearity)
* The [Electronic Control Unit](https://en.wikipedia.org/wiki/Electronic\_Control\_Unit) (ECU) under test is connected to the system and stimulated by a set of vehicle maneuvers executed by the simulator

<figure><img src="https://in.mathworks.com/discovery/hardware-in-the-loop-hil/_jcr_content/mainParsys/image.adapt.full.medium.jpg/1692124217139.jpg" alt=""><figcaption><p>HiL system</p></figcaption></figure>
