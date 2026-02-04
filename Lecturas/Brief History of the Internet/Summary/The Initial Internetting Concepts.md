# The Shift to Open Architecture Networking

By 1972, the focus shifted from building a single network (ARPANET) to connecting multiple independent networks (satellite, ground radio, and cable) of arbitrary design. This led to the concept of **Open Architecture Networking**.
## 1. The Core Philosophy: "Internetting"
Introduced by **Bob Kahn** at DARPA, the "Internetting" program was designed to allow different network technologies to interwork through a meta-level "Internetworking Architecture."
### Traditional vs. Open Architecture
* **Traditional (Circuit Switching):** Networks interconnect at the circuit level, passing bits on a synchronous basis.
* **Open Architecture:** Individual networks are separately designed. They act as **peers** rather than components of one another. No specific internal changes are required for a network to join the Internet.
## 2. The Birth of TCP/IP
The original protocol, **NCP (Network Control Protocol)**, was insufficient because it relied on the ARPANET's internal reliability. Bob Kahn and **Vint Cerf** teamed up in 1973 to design a new protocol: **TCP/IP**.
### Kahn’s Four Ground Rules
1. **Autonomy:** Each network stands on its own; no internal changes required to connect.
2. **Best-Effort Delivery:** If a packet fails, the source retransmits it. No reliability is guaranteed by the network itself.
3. **Gateways/Routers:** Simple "black boxes" connect networks. They store no information about individual packet flows to avoid complex recovery modes.
4. **No Global Control:** Decentralized operations at the global level.
### Key Technical Breakthroughs
* **32-bit Addressing:** Initially assumed 256 networks (8 bits) and 16 million hosts (24 bits) would be sufficient.
* **Sliding Windows:** Used for flow control and cumulative acknowledgments (ACKs).
* **Octet Streams:** Communication was treated as a long stream of bytes (octets).
## 3. The Great Split: TCP, IP, and UDP
Originally, there was only one protocol: **TCP**. However, as advanced applications like **Packet Voice** emerged in the 1970s, it became clear that total reliability (retransmitting every lost packet) was not always desirable.

The protocol was reorganized into three distinct layers:
* **IP (Internet Protocol):** Handles basic addressing and forwarding of individual packets.
* **TCP (Transmission Control Protocol):** Provides a reliable, sequenced "virtual circuit" (perfect for File Transfer and Telnet).
* **UDP (User Datagram Protocol):** Provides direct access to IP for applications that prefer speed over reliability (perfect for voice/video).
## 4. Resource Sharing & The "Killer App"
While the Internet was built for **resource sharing** (accessing expensive time-sharing systems), its true impact was social:

* **Email:** Changed the nature of collaboration and was instrumental in building the Internet itself.
* **General Infrastructure:** Unlike previous systems, the Internet was not designed for a single application. Its general-purpose nature (TCP/IP) allowed for the later emergence of the **World Wide Web**, **Internet Telephony**, and **Cloud Computing**.
##  Source Archive: Open Architecture

> [!quote] 
> (Full text from your prompt is archived here...)
> "The original ARPANET grew into the Internet. Internet was based on the idea that there would be multiple independent networks of rather arbitrary design... [text continues] ...general purpose nature of the service provided by TCP and IP that makes this possible."
## Timeline Addition
- **1972:** Bob Kahn introduces Open Architecture/Internetting at DARPA.
- **1973 (Spring):** Kahn and Vint Cerf collaborate on the detailed TCP design.
- **1973 (Sept):** First version of the TCP/IP approach presented at Sussex University.
- **Late 1970s:** TCP split into TCP and IP; UDP added to support real-time applications.