
 # Networking

<details>
<summary>What is HTTP?</summary>

The Hypertext Transfer Protocol (HTTP) is the foundation of the World Wide Web, and is used to load webpages using hypertext links. HTTP is an application layer protocol designed to transfer information between networked devices and runs on top of other layers of the network protocol stack. A typical flow over HTTP involves a client machine making a request to a server, which then sends a response message.

HTTPS is an extension of the Hypertext Transfer Protocol. The S in HTTPS stands for “secure.” When a website is encrypted with TLS (or SSL), it uses Hypertext Transfer Protocol Secure (HTTPS). 

Basically, it’s HTTP with encryption. It is used to secure communication over a computer network and is widely used on the Internet. HTTPS encrypts and decrypts user page requests and the pages returned by the web server.

</details>

<details>
<summary>Difference between HTTP and HTTPS?</summary>

The most significant difference between the two protocols is that HTTPS is encrypted and secured using digital certificates, while HTML is not. When you visit a website using HTTPS, your connection to that site is encrypted. Any information you send or receive on that site is also encrypted.

Another difference between the protocols is that HTTPS uses port 443, while HTML uses port 80. Port 443 is the standard port for secured Hypertext Transfer Protocol (HTTPS). Port 80 is the default port for unsecured Hypertext Transfer Protocol.


</details>

<details>
<summary>How does a typical HTTP request look like?</summary>

An HTTP request is the way Internet communications platforms such as web browsers ask for the information they need to load a website.

Each HTTP request made across the Internet carries with it a series of encoded data that carries different types of information. A typical HTTP request contains:

1) HTTP version type
2) a URL
3) an HTTP method
4) HTTP request headers
5) Optional HTTP body

</details>

<details>
<summary>What is an HTTP method?</summary>

An HTTP method, sometimes referred to as an HTTP verb, indicates the action that the HTTP request expects from the queried server. For example, two of the most common HTTP methods are ‘GET’ and ‘POST’; a ‘GET’ request expects information back in return (usually in the form of a website), while a ‘POST’ request typically indicates that the client is submitting information to the web server (such as form information, e.g. a submitted username and password).

</details>

<details>
<summary>What are HTTP request headers?</summary>

HTTP headers contain text information stored in key-value pairs, and they are included in every HTTP request. These headers communicate core information, such as what browser the client is using and what data is being requested.

</details>

<details>
<summary>What is in an HTTP request body?</summary>

The body of a request is the part that contains the ‘body’ of information the request is transferring. The body of an HTTP request contains any information being submitted to the web server, such as a username and password, or any other data entered into a form.

</details>

<details>
<summary>What is in an HTTP response?</summary>

An HTTP response is what web clients (often browsers) receive from an Internet server in answer to an HTTP request. These responses communicate valuable information based on what was asked for in the HTTP request.

A typical HTTP response contains:

1) An HTTP status code
2) HTTP response headers
3) Optional HTTP body

</details>

<details>
<summary>What’s an HTTP status code?</summary>

HTTP status codes are 3-digit codes most often used to indicate whether an HTTP request has been successfully completed. Status codes are broken into the following 5 blocks:

- 1xx Informational
- 2xx Success
- 3xx Redirection
- 4xx Client Error
- 5xx Server Error

The “xx” refers to different numbers between 00 and 99.

Status codes starting with the number ‘2’ indicate a success. For example, after a client requests a webpage, the most commonly seen responses have a status code of ‘200 OK’, indicating that the request was properly completed.

If the response starts with a ‘4’ or a ‘5’ that means there was an error and the webpage will not be displayed. A status code that begins with a ‘4’ indicates a client-side error (it is very common to encounter a ‘404 NOT FOUND’ status code when making a typo in a URL). A status code beginning in ‘5’ means something went wrong on the server side. Status codes can also begin with a ‘1’ or a ‘3’, which indicate an informational response and a redirect, respectively.

</details>

<details>
<summary>What are HTTP response headers?</summary>

Much like an HTTP request, an HTTP response comes with headers that convey important information such as the language and format of the data being sent in the response body.

</details>

<details>
<summary>What is in an HTTP response body?</summary>

Successful HTTP responses to ‘GET’ requests generally have a body which contains the requested information. In most web requests, this is HTML data that a web browser will translate into a webpage.

</details>

<details>
<summary>TCP vs UDP</summary>

Protocols are rules that govern how data is formatted and sent over a network. TCP and UDP are two different methods for doing the same job: transferring data via the internet. They enable servers and devices to communicate so you can send emails, watch Youtube, play games, and browse web pages.

The main difference between TCP (transmission control protocol) and UDP (user datagram protocol) is that TCP is a connection-based protocol and UDP is connectionless. While TCP is more reliable, it transfers data more slowly. UDP is less reliable but works more quickly. This makes each protocol suited to different types of data transfers.

</details>

<details>
<summary>What is DNS?</summary>

The process of DNS resolution involves converting a hostname (such as www.google.com) into a computer-friendly IP address (such as 192.168.1.1). An IP address is given to each device on the Internet, and that address is necessary to find the appropriate Internet device - like a street address is used to find a particular home. When a user wants to load a webpage, a translation must occur between what a user types into their web browser (example.com) and the machine-friendly address necessary to locate the example.com webpage.

</details>

<details>
<summary>How does DNS work?</summary>


DNS (Domain Name System) works by translating human-friendly domain names (like www.example.com) into IP addresses (like 192.168.1.1) that computers use to identify each other on the internet. Here's a simplified step-by-step process:

1. User enters a domain name in a web browser.
2. The computer first checks its local DNS cache to see if it already knows the corresponding IP address.
3. If not found, the computer sends a DNS query to a DNS resolver (usually provided by your internet service provider or a public DNS service like Google's 8.8.8.8).
4. The DNS resolver searches its cache for the IP address. If not found, it starts a recursive process:
  a. The resolver queries root DNS servers to find the authoritative DNS server for the top-level domain (like .com).
  b. The resolver then queries the top-level domain's authoritative DNS server to find the authoritative server for the specific domain (like example.com).
  c. Finally, the resolver queries the domain's authoritative server for the IP address of the requested domain (www.example.com).
1. The authoritative DNS server responds with the IP address, and the resolver caches this information for future use.
2. The resolver returns the IP address to the user's computer.
3. The computer can now establish a connection with the web server at the provided IP address, allowing the user to access the website associated with the domain name.

- In essence, DNS acts as the internet's phone book, translating user-friendly domain names into the numerical addresses computers need to communicate.

</details>

<details>
<summary>What is TLS?</summary>

TLS (Transport Layer Security) is a cryptographic protocol that provides secure communication over a computer network, such as the internet. It ensures data privacy and integrity by encrypting the data transmitted between two systems, typically a web browser and a web server. TLS is commonly used to secure online transactions, like credit card payments and sensitive data transfers, by establishing a secure, encrypted connection between the client and server. This encryption helps protect against eavesdropping and data tampering during transmission.

</details>

<details>
<summary>What are CIDR ranges?</summary>

CIDR (Classless Inter-Domain Routing) ranges are a way to represent and allocate IP addresses and subnets in a more flexible manner than traditional subnetting using classes (Class A, B, C, etc.). In CIDR notation, an IP address is followed by a slash ("/") and a number, which indicates the number of bits in the network portion of the address. Here's a simple example:

IP Address: 192.168.1.0
CIDR Notation: 192.168.1.0/24
In this example, "/24" means that the first 24 bits of the IP address are used to identify the network, leaving 8 bits for host addresses. This allows for finer control over IP address allocation and subnetting compared to the older class-based system (e.g., Class A, B, C).

CIDR notation is widely used in networking to specify IP address ranges, making it easier to manage and allocate IP addresses efficiently.

</details>

<details>
<summary>What is ingress and egress traffic?</summary>

In networking and security, "ingress" and "egress" refer to the movement of data or traffic into and out of a network, system, or device:

**Ingress Traffic:** This is incoming traffic that enters a network or system. Ingress traffic typically originates from external sources, such as the internet, and flows into a network through a gateway, router, or firewall. Monitoring and controlling ingress traffic is important for security purposes to prevent unauthorized access or attacks.

**Egress Traffic:** Egress traffic, on the other hand, is outgoing traffic that exits a network or system and goes towards external destinations. Egress traffic might include data leaving a corporate network to access a website, send emails, or communicate with cloud services. Managing egress traffic is essential for monitoring data leaving a network and enforcing policies related to data transmission.

In summary, ingress traffic comes into a network, while egress traffic goes out of it. Network administrators often use firewall rules and security measures to control and secure both ingress and egress traffic to protect the network from threats and ensure proper data flow.

</details>

<details>
<summary>What is a switch vs a hub?</summary>

A switch and a hub are both networking devices used to connect multiple devices in a local area network (LAN), but they operate in fundamentally different ways:

**Switch:**

A switch operates at the data link layer (Layer 2) of the OSI model.
It is an intelligent device that examines the MAC (Media Access Control) addresses of data packets to determine where to forward them.
Switches create a dedicated, point-to-point connection between the sender and recipient, improving network efficiency by reducing collisions.
They can filter and forward traffic only to the specific device that needs it, enhancing network security and performance.
Switches are common in modern networks due to their efficiency and ability to handle high traffic loads.

**Hub:**

A hub operates at the physical layer (Layer 1) of the OSI model.
It is a basic and passive device that simply broadcasts incoming data packets to all connected devices without any intelligence.
Hubs do not examine MAC addresses or make decisions about where to send data; they indiscriminately send data to all connected devices.
This broadcasting approach can lead to network congestion and collisions, especially in larger networks.
Hubs are considered outdated and inefficient for modern networks, and they are rarely used today.
In summary, switches are more advanced and efficient networking devices that intelligently forward data packets to the appropriate recipient, while hubs are basic and outdated devices that broadcast data to all connected devices, leading to less efficient network communication. Switches are the preferred choice for building modern, high-performance LANs.

</details>

<details>
<summary>What is a switch vs a router?</summary>

**Switch:**

A switch operates at the data link layer (Layer 2) of the OSI model.
It is used to connect devices within a local area network (LAN).
Switches make forwarding decisions based on MAC (Media Access Control) addresses and create efficient, dedicated connections between devices within the same LAN.
They are primarily used for local traffic management and do not have a role in routing traffic between different networks.

**Router:**

A router operates at the network layer (Layer 3) of the OSI model.
It connects different networks together and directs traffic between them.
Routers use IP addresses to make routing decisions, determining the most appropriate path for data packets to reach their destination, whether that destination is within the same local network or in a different network (e.g., the internet).
Routers are essential for interconnecting multiple LANs and facilitating communication between devices on different networks.
In summary, switches are used for local network traffic management within a single LAN, while routers are used to connect and route traffic between different networks, including routing traffic between LANs and the broader internet. Both devices play critical roles in network communication and connectivity.

</details>

<details>
<summary>What is HTTPS vs Websockets?</summary>

HTTPS and WebSockets are both protocols used for web communication, but they serve different purposes and operate in distinct ways:

**HTTPS (HyperText Transfer Protocol Secure):**

- HTTPS is an extension of the HTTP protocol used for secure communication over the internet.
It encrypts the data transmitted between a web browser and a web server, providing data confidentiality and integrity.
- HTTPS uses SSL/TLS (Secure Sockets Layer/Transport Layer Security) to establish a secure, encrypted connection between the client and server.
- It is commonly used for secure web browsing, online transactions, and protecting sensitive data, such as login credentials and personal information.
- HTTPS is a request-response protocol, meaning that the client sends a request to the server, and the server responds with the requested data.

**WebSockets:**
- WebSockets is a protocol that provides full-duplex communication channels over a single TCP connection.
Unlike HTTP(S), which is request-response-based and stateless, WebSockets allow for two-way, real-time communication between a client (e.g., a web browser) and a server.
- WebSockets are often used in applications that require real-time updates, such as chat applications, online gaming, collaborative tools, and live data feeds.
- They are more efficient for scenarios where continuous communication is needed, as they eliminate the need for repeatedly establishing new connections.
- WebSockets allow data to be pushed from the server to the client and vice versa without the overhead of frequent HTTP requests.

In summary, HTTPS is a protocol for securing web communication, while WebSockets provide a framework for real-time, bidirectional communication over a single, long-lived connection. They are used for different purposes but can complement each other in web applications, where secure and real-time communication is required.

</details>

<details>
<summary>Explain how a 3 way handshake works?</summary>

A three-way handshake is a method used in a TCP/IP network to create a connection between a host and a client. It’s called a three-way handshake because it is a three-step method in which the client and server exchanges packets. The three steps are as follows: The client sends a SYN(Synchronize) packet to the server check if the server is up or has open ports. The server sends SYN-ACK packet to the client if it has open ports. The client acknowledges this and sends an ACK(Acknowledgment) packet back to the server.

</details>

<details>
<summary>Stateless vs Stateful firewalls?</summary>

Stateless and stateful firewalls are two types of network security devices that filter and control incoming and outgoing network traffic, but they do so in different ways:

**Stateless Firewall:**

- Stateless firewalls filter traffic based solely on the source and destination IP addresses, as well as port numbers.
They do not maintain any information about the state of ongoing network connections.
- Stateless firewalls are simpler and faster but lack the ability to make decisions based on the context or state of a connection.
- Each packet is evaluated in isolation, without considering whether it's part of an established connection or whether it's a legitimate response to an outbound request.
- Stateless firewalls are often used in basic network security setups and are suitable for scenarios where a basic level of security is sufficient.

**Stateful Firewall:**

- Stateful firewalls, also known as dynamic packet filtering firewalls, maintain a table of the state of active network connections.
- They keep track of the state of TCP and UDP sessions, including the state of each connection (e.g., established, related, new) and their associated ports.
- Stateful firewalls make decisions based on the context of network traffic, allowing them to permit or deny packets based on whether they are part of a legitimate, established connection.
- This context-awareness makes stateful firewalls more effective at protecting against various types of attacks, such as port scanning and certain forms of packet-level attacks.
- They are commonly used in enterprise networks and provide a higher level of security compared to stateless firewalls.

In summary, stateless firewalls filter traffic based solely on basic information like IP addresses and port numbers, while stateful firewalls maintain information about the state of active connections and make decisions based on the context of the traffic. Stateful firewalls are generally more advanced and provide better security for modern network environments.

</details>

<details>
<summary>What are VPCs?</summary>

VPC stands for Virtual Private Cloud. It is a fundamental component of cloud computing infrastructure, particularly in services like Amazon Web Services (AWS) and Microsoft Azure.

**VPC (Virtual Private Cloud):**

- A VPC is a logically isolated section of a cloud provider's network where you can launch and manage your virtual resources like virtual machines (VMs), databases, and storage.
- It allows you to create your own private network within the cloud, complete with private IP addresses, subnets, route tables, and security groups.
- VPCs provide control over network configurations, security, and communication between resources, making it possible to build secure and scalable cloud-based applications.
- You can also connect your VPC to your on-premises data centers or other VPCs, creating a hybrid or multi-cloud network.
- VPCs are essential for ensuring network isolation, security, and resource organization in cloud environments.

</details>

<details>
<summary>What is subnetting?</summary>

Subnetting is the process of dividing a larger IP network into smaller, more manageable subnetworks, or "subnets." This practice is commonly used in networking to:

- Improve Network Efficiency: Subnetting allows you to create smaller segments within a larger network. This can help reduce broadcast traffic and improve overall network performance by isolating traffic to specific subnets.

- Enhance Security: By dividing a network into subnets, you can implement access control lists (ACLs) and firewall rules more effectively. This helps control and secure traffic between different parts of the network.

- IP Address Management: Subnetting aids in efficient IP address allocation. Each subnet can have its own range of IP addresses, making it easier to manage and allocate IP addresses within an organization.

- Isolation and Segmentation: Subnets can isolate different types of devices or services from each other. For example, you can place servers in one subnet and user devices in another to improve security and management.

Subnetting involves dividing an IP address range into smaller, contiguous blocks, each with its own network address and a range of host addresses. This is typically done by modifying the subnet mask associated with the IP address range. The subnet mask designates which portion of the IP address is the network part and which part is the host part.

For example, if you have the IP address range 192.168.0.0/24 (where "/24" indicates a subnet mask of 255.255.255.0), you can subnet it into smaller subnets like 192.168.0.0/25 and 192.168.0.128/25, each with half of the original IP address range's available host addresses.


</details>

<details>
<summary>What is DHCP?</summary>


DHCP stands for Dynamic Host Configuration Protocol. It is a network protocol used to automate and simplify the process of assigning IP addresses and other network configuration settings to devices on a local network.

**DHCP (Dynamic Host Configuration Protocol):**

- DHCP is a client-server protocol commonly used in local area networks (LANs) and on the internet.
- It eliminates the need for manual IP address configuration on each device in a network.
- When a device (client) connects to a network, it sends a DHCP request to a DHCP server, typically a router or dedicated DHCP server.
- The DHCP server responds with an available IP address, subnet mask, default gateway, DNS server addresses, and other configuration parameters.
- The client then configures itself with the provided information, making it ready to communicate on the network.

</details>

