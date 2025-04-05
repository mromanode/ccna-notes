1. What is a networking model in networking?
	- A networking model, sometimes also called either a _networking architecture_ or _networking blueprint_, refers to a comprehensive set of documents.
2. <mark style="background: #FF5582A6;">Individually, what each document describe?</mark>
	- Each document describes one small function required for a network.
3. collectively, what these document define?
	- Collectively, these documents define everything that should happen for a computer network to work.
4. What is a protocol, defined by some documents?
	- Is a set of logical rules that devices must follow to communicate.
5. <mark style="background: #FF5582A6;">Which are the physical requirements defined by others documents?</mark>
	- A document could define the voltage and current levels used on a particular cable when transmitting data.
6. What is the networking model used today?
	- TCP/IP.
7. What ISO stand for?
	- International Organization for Standardization
8. What model ISO does created?
	- OSI.
9. What OSI stand for?
	- Open Systems Interconnection.
10. <mark style="background: #FF5582A6;">What was the noble goal of the Open Systems Interconnection (OSI) model?</mark>
	- To standardize data networking protocols to allow communication among all computers across the entire planet.
11. What DoD stand for?
	- U.S. Departement of Defense
12. What model DoD does created 
	- A model called TCP/IP.
13. <mark style="background: #FF5582A6;">What the TCP/IP model defines and references that allow computers to communicate</mark>
	- The TCP/IP model both defines and references a large collection of protocols that allow computers to communicate. 
14. By using what, TCP/IP define a protocol?
	- To define a protocol, TCP/IP uses documents called Requests For Comments (RFC).
15. <mark style="background: #FF5582A6;">What each layer of the TCP/IP does define to create a working communication system</mark>?
	- Each layer broadly defines a set of functions that helps create a working communication system.
16. <mark style="background: #FF5582A6;">What RFC gives at each layer of the TCP/IP model?</mark>
	- Each RFC gives the specifics about an option to implement one or more of the functions at some layer of the model.
17. <mark style="background: #FF5582A6;">How the TCP/IP model does to avoid repeating work already done?</mark>
	- The TCP/IP model also avoids repeating work already done by some other standards body or vendor consortium by simply referring to standards or protocols created by those groups. For example, the Institute of Electrical and Electronics Engineers (IEEE) defines Ethernet LANs; the TCP/IP model does not define Ethernet in RFCs, but refers to IEEE Ethernet as an option.
18. <mark style="background: #FF5582A6;">What IEEE stand for?</mark>
	- Institute of Electrical and Electronics Engineers
19. What NIC stand for?
	- Network Interface Card
20. <mark style="background: #FF5582A6;">What does the NIC implements in the Physical layer and Data-Link layer?</mark>
	- Implement the standards for both layer to support physical communications.
21.  <mark style="background: #FF5582A6;">What the OS in the computer implements?</mark>
	- The OS on the computer implements protocols from the network and transport layers.
22. <mark style="background: #FF5582A6;">What the web browser does implements?</mark>
	- The web browser implements some application layer protocols (for instance, HTTP or HTTPS.)
23. What the Physical layer focuses on?
	- The physical layer focuses on how to transmit bits over each link. 
24. <mark style="background: #FF5582A6;">What the Data-Link layer focuses on?</mark>
	- The data-link layer focuses on the rules that control the use of the physical link.
25. What the Network layer focuses on?
	- The network layer focuses on delivering data over the entire path from the original sending computer to the final destination computer.
26. What the Transport layer and the Application layer focus on?
	- The top two layers focus more on the applications that need to send and receive data. For instance, how to identify data, how to ask for the data to be sent, and how to recover the data if lost in transmission.
27. What are the common protocols for each layers?
	- Application: HTTPS, POP3, SMTP
	- Transport: TCP, UDP
	- Network: IP, ICMP
	- Physical & Data-Link: Ethernet, 802.11 (Wi-Fi)
28. What the Application layer provides services to?
	- To the software running on a computer.
29. What the Application layer does define?
	- Defines services that applications need. For example, application protocol HTTP defines how web browsers can pull the contents of a web page from a web server. 
30. What HTTP stand for?
	- Hypertext Transfer Protocol.
31. What HTTP is used for?
	- To request files from the server and giving the server a way to return the content of those files.
32. Which protocol does HTTP use?
	- TCP/IP
33. What is the Header in a protocol?
	- A place to put information used by that protocol.
34. How HTTP work?
	1. Bob (Web Browser) send a request with an HTTP header. This HTTP header contains a request to "GET" a file. The request typically contains the name of the file. If no file is mentioned, the web server assumes that Bob wants the default web page.
	2. Larry (Web Server) returns a message with an http header, containing a return code (200) which means "OK" returned in the header. 
	3. HTTP transfers the data by sending multiple messages, each with a part of the file. Rather than wasting space by sending repeated HTTP headers that list the same information, these additional messages simply omit the header.
35. What are the most common protocol used in the Transport Layer by the TCP/IP model?
	- The two most commonly used transport layer protocols are the Transmission Control Protocol (TCP) and the User Datagram Protocol (UDP).
36. Which layer does the Transport Layer provides service to in the TCP/IP model?
	- Transport layer protocols provide services to the application layer protocols that reside one layer higher in the TCP/IP model.
37. What each layer provide to the layer above it?
	-  Each layer provides a service to the layer above it.
38. How is called the concept of error recovering provided by the TCP protocol in the TCP/IP model?
	- Acknowledgment
39. What is an example of TCP Error Recovery service as Provided to HTTP?
	1.  Along the HTTP header, there is also a TCP Header. The TCP header shows a sequence number (SEQ) with each message.
	2. If the network has a problem, and the network fails to deliver the TCP message (called a segment) with a sequence number 2, when Bob receives messages with sequence numbers 1 and 3, but does not receive a message with sequence number 2, Bob realizes that message 2 was lost. That realization by Bob’s TCP logic causes Bob to send a TCP segment back to Larry, asking Larry to send message 2 again.
40. How does the concept of Adjacent-Layer Interaction works?
	- The higher-layer protocol uses the next lower-layer protocol to perform the service.
41. How does the concept of Same-Layer Interaction works?
	- When a particular layer on one computer wants to communicate with the same layer on another computer, the two computers use headers to hold the information that they want to communicate. 
42. What are the most common protocols used in the Network layer by the TCP/IP model?
	- TCP and IP
43. What features IP does provide in the TCP/IP model?
	- Addressing and Routing.
44. Why IP defines addresses in the TCP/IP model?
	- First, each device that uses TCP/IP—each TCP/IP _host_—needs a unique address so that it can be identified in the network. IP also defines how to group addresses together.
45. How the style of a IP is called?
	- Dotted Decimal Notation (DDN)
46. What are routers and what is their purpose?
	- Routers are networking devices that connect the parts of the TCP/IP network together for the purpose of routing (forwarding) IP packets to the correct destination.
47. What are the 3 steps of IP Forwarding?
	- Step 1, begins with Larry being ready to send an IP packet. Larry’s IP process chooses to send the packet to some router—a nearby router on the same LAN—with the expectation that the router will know how to forward the packet. Larry doesn’t need to know anything more about the topology or the other routers.
	- At Step 2, Router R1 receives the IP packet, and R1’s IP process makes a decision. R1 looks at the destination address (2.2.2.2), compares that address to its known IP routes, and chooses to forward the packet to Router R2. This process of forwarding the IP packet is called _IP routing_ (or simply _routing_).
	- At Step 3, Router R2 repeats the same kind of logic used by Router R1. R2’s IP process will compare the packet’s destination IP address (2.2.2.2) to R2’s known IP routes and make a choice to forward the packet to the right, on to Bob.
48. What the physical layer does define?
	- The physical layer defines the cabling and energy (for example, electrical signals) that flow over the cables.
49. What are the 4 steps of a networking device sending an IP packet to a router?
	- Larry encapsulates the IP packet between an Ethernet header and Ethernet trailer, creating an Ethernet frame.
	- Larry physically transmits the bits of this Ethernet frame, using electricity flowing over the Ethernet cabling.
	- Router R1 physically receives the electrical signal over a cable and re-creates the same bits by interpreting the meaning of the electrical signals.
	- Router R1 de-encapsulates the IP packet from the Ethernet frame by removing and discarding the Ethernet header and trailer.
50. What the term encapsulation refers to?
	- The term encapsulation refers to the process of putting headers (and sometimes trailers) around some data.
51. What are the 5 steps of encapsulation
	1. Create and encapsulate the application data with any required application layer headers. For example, the HTTP OK message can be returned in an HTTP header, followed by part of the contents of a web page.
	2. Encapsulate the data supplied by the application layer inside a transport layer header. A TCP or UDP header is typically used.
	3. Encapsulate the data supplied by the transport layer inside a network layer (IP) header. IP defines the IP addresses that uniquely identify each computer.
	4. Encapsulate the data supplied by the network layer inside a data-link layer header and trailer. This layer uses both a header and a trailer.
	5. Transmit the bits. The physical layer encodes a signal onto the medium to transmit the frame.
52. For each layer message, what is their term in the TCP/IP model?
	- Application: Data
	- Transport: Segment
	- Network: Packet
	- Data-Link: Frame
53. How many layers does the OSI model have compared to the TCP/IP (Common) and the TCP/IP (1122)
	- OSI: 7
		- Application
		- Presentation
		- Session
		- Transport
		- Network
		- Data-Link
		- Physical
	- TCP/IP (Common):
		- Application
		- Transport
		- Network
		- Data-Link
		- Physical
	- TCP/IP (RFC 1122):
		- Application
		- Transport
		- Internet
		- Link