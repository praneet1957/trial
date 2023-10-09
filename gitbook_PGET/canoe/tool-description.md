# Tool description

**Diagnostic ISO/ TP Tab** - Find all networks, CAN, LIN, MOST etc..

Diagnostic description file ex: CDD file

* diagnostic session -- connect manually to ECU -- changing configuration
  * ST min - time between frame, Block Size, Flow control, Max data size
* tester for extended diagnostic session -- client time & interval
  * Client time, Server time, Timeout for ECU to respond, Extended time out

Ref [https://www.youtube.com/watch?v=6DK7OQD9\_pU\&list=PLYiraB-Sgw6tbIfjQtrfIx3g70j\_wdTV1](https://www.youtube.com/watch?v=6DK7OQD9\_pU\&list=PLYiraB-Sgw6tbIfjQtrfIx3g70j\_wdTV1)

**Diagnostic Fault memory panel**

* All the fault memory list of an ECU&#x20;
  * tester present behavior&#x20;
  * updating fault memory read frequency - cyclic update
  * DTC- Diagnostic trouble codes
  * reading faults, properties, true means fault has occurred

**CAN message transmission using CAPL**

simulation setup -> Networks -> CAN --> CAN database file&#x20;

CAPL code to initiate on key 'a' and timer.  &#x20;

**System and communication window**

system configuration -> application models -> system explorer

**DoIP - communication sequence**

* IP address configuration and assignment
* Vehicle identification request & response using UDP protocol
* TCP is used, routing request for ECU, exchange of diagnostic messages

**Trace Window**

identical time stamp - same msg,&#x20;



