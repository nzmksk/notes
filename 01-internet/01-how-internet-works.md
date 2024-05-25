# Contents
- [Introduction to the Internet](#introduction-to-the-internet)
- [Where is the Internet?](#where-is-the-internet)
- [Who Runs the Internet?](#who-runs-the-internet)
- [How the Internet Works](#how-the-internet-works)
- [How Wireless Internet Works](#how-wireless-internet-works)
- [What is the Cloud?](#what-is-the-cloud)
- [IPv6](#ipv6)
- [Building Applications with TCP/IP](#building-applications-with-tcpip)
- [Securing Internet Communication with SSL/TLS](#securing-internet-communication-with-ssltls)
- [Glossary](#glossary)

## Introduction to the Internet
- Began as ARPANET, an academic research network
- Developed in 1969 to create a decentralized communication network that could withstand a **nuclear attack**
- Funded by US military's Advanced Research Projects Agency (ARPA)
- In 1973, software engineers **Vint Cerf** and **Bob Kahn** began work on the next generation of networking standards for ARPANET
- The standards, known as **TCP/IP**, became the foundation of the modern internet
- ARPANET switched to using TCP/IP on 1st January, 1983
- During 1980s, funding for the internet shifted from the military to **National Science Foundation**
- NSF funded the long-distance networks that as the internet's backbone from 1981 - 1994
- Became a global commercial network in the 1990s
- US government turned control over the internet backbone to the private sector in 1994

## Where is the Internet?
Consist of 3 parts:
- **Last mile** - part of the internet that connects homes and small businesses to the internet. Also includes the towers that allow people to access the internet with their cell phones.
- **Data centres** - rooms full of servers that store user data and host online apps and content. Data centers have very fast internet connections, allowing them to serve many users simultaneously. They are often located in remote areas where land and electricity are cheap.
- **Backbone** - consists of long-distance networks - mostly on fiber optic cables that carry data between data centers and consumers.

## Who Runs the Internet?
- Is a decentralized network of networks
- The shared technical standards that make the internet work are managed by **Internet Engineering Task Force (IETF)**
- IETF is an open organization - anyone is free to attend meetings, propose new standards, and recommend changes to existing standards
- It's not required to adopt standards endorsed by IETF, but IETF-consensus-based decision-making process helps to ensure that its recommendations are generally adopted by the internet community
- **Internet Corporation for Assigned Names and Numbers (ICANN)** is responsible for internet governance
- ICANN is in charge of distributing domain names and IP addresses, though doesn't control who can connect to the internet or what kind of information can be sent over it

## How the Internet Works
- The core of the internet is a global network of interconnected routers
- When data is sent over the internet, it is broken up into small packets
- The router examines the packet and forwards it to the next router in the path towards its destination
- The process continues until the packet reaches its final destination
- IP and TCP ensure packets are sent and received correctly

## How Wireless Internet Works
| WiFi | Cellular |
| --- | --- | 
| Use unlicensed spectrum - electromagnetic frequencies that are available for anyone to use without charge. | More centralized, work by breaking up the service territory into cells. In the densest areas, cells can be as small as a single city block and miles across in rural areas. |
| Strict limits on the power and range of wifi networks to prevent neighbours' networks from interfering with each other. | Each cell has a tower as its centre providing services. When a device moves from one cell to another, the network automatically hands off the device from one tower to another. |

## Packet
- Basic unit of information transmitted over the internet.
- Allow the network's capacity to be used more efficiently.
- Consists of two parts:
  - Header - contains information that helps the packet get to its destination, including the length of the packet, its source and destination, and a checksum value that helps the recipient detect if a packet was damaged in transit.
  - Body - contains the actual data being sent.
- A packet can contain up to 64 kb of data, which is roughly 20 pages of plain text.

## IPv6
- The current internet standard, known as IPv4, only allows for about 4 billion IP addresses
- This was considered a very big number in the 1970s, but today, the supply of IPv4 addresses is nearly exhausted
- Internet engineers have developed a new standard called IPv6 that allows for at least 100 undecillion (one followed by 38 zeros) unique addresses

## Building Applications with TCP/IP
- TCP/IP is the underlying communication protocol used by most internet-based applications and services
- Provides a reliable, ordered, and error-checked delivery of data between applications running on different devices
- Key concepts to understand:

| Term | Description |
| --- | --- |
| Port | Used to identify the application or service running on a device. Each application or service is assigned a unique port number, allowing data to be sent to the correct destination. |
| Socket | A combination of IP address and a port number, representing a specific endpoint for communication. Used to establish connections between devices and transfer data between applications. |
| Connection | Established between two sockets when two devices want to communicate with each other. During the connection establishment process, the devices negotiate various parameters such as the maximum segment size and window size, which determine how data will be transmitted over the connection. |
| Data transfer | Once a connection is established, data can be transferred between applications running on each device. Data is typically transmitted in segments, with each segment containing a sequence number and other metadata to ensure reliable delivery. |
- Communication between computers is accomplished through the use of protocol stack.

| Protocol | Stack |
| --- | --- |
| Application Protocols Layer | Protocols specific to applications such as WWW, e-mail, FTP, etc. |
| Transmission Control Protocol (TCP) Layer | TCP directs packets to a specific application on a computer using a port number. |
| Internet Protocol (IP) Layer | IP directs packets to a specific computer using an IP address |
| Hardware Layer | Converts binary packet data to network signals and back. Examples are ethernet network card, modem for phone lines, etc. |

## Securing Internet Communication with SSL/TLS
- SSL and TLS are protocols used to encrypt data being transmitted over the internet
- Commonly used to provide secure connections for applications such as web browsers, email clients, and file transfer programs
- Few key concepts to understand:

| Term | Description |
| --- | --- |
| Certificate | SSL/TLS certificates are used to establish trust about the client and server. They contain information about the identity of the server and are signed by a trusted third party (a Certificate Authority) to verify their authenticity. |
| Handshake | During the SSL/TLS handshake process, the client and server exchange information to negotiate the encryption algorithm and other parameters for the secure connection. |
| Encryption | Once the secure connection is established, data is encrypted using the agreed-upon algorithm and other parameters for the secure connection. |
- Ensure that your application is designed to use SSL/TLS when transmitting sensitive data such as login credentials, payment information, and other personal data
- Also ensure you obtain and maintain valid SSL/TLS certificates for your servers

## Glossary
| Term | Description |
| --- | --- |
| 5G | The latest generation of mobile network technology, offering faster speeds, lower latency, and greater capacity than previous generations. It is expected to enable new use cases and applications, such as autonomous vehicles and remote surgery. |
| Artificial Intelligence (AI) | AI technologies such as machine learning and natural language processing are already being used to power a wide range of applications and services, from voice assistants to fraud detection. It is expected to enable new use cases and transform industries such as healthcare, finance, and education. |
| Blockchain | A distributed ledger technology that enables secure, decentralized transactions. It is being used to power a wide range of applications, from cryptocurrency to supply chain management. |
| Cloud Computing | Delivery of computing services - including servers, storage, databases, networking, software, analytics, and intelligence over the internet (*the cloud*) to offer faster innovation, flexible resources, and economies of scale. |
| Domain Name | A human-readable name that is used to identify a website, such as google.com |
| Domain Name System (DNS) | Responsible for translating domain names into IP addresses |
| Edge Computing | Refers to the processing and storage of data at the edge of the network, rather than in centralized data centers. It is expected to enable new use cases and applications, such as real-time analytics and low-latency applications. |
| Hypertext Transfer Protocol (HTTP) | Used to transfer data between a client (e.g. web browser) and a server (e.g. website) |
| Hypertext Transfer Protocol Secure (HTTPS) | An encrypted version of HTTP using SSL/TLS encryption |
| IP Address | A unique identifier assigned to each device on a network, used to route data to the correct destination |
| Internet | A network of networks |
| Internet of Things (IoT) | Refers to the network of physical devices, vehicles, home appliances, and other objects that are connected to the internet and can exchange data. It is expected to revolutionize industries such as healthcare, transportation, and manufacturing. |
| Internet Protocol (IP) | Responsible for routing packets to their correct destination |
| Network | A group of computers or other devices connected to each other |
| Packet | A small unit of data that is transmitted over the internet |
| Router | Responsible for directing traffic between different devices and systems |
| Secure Sockets Layer (SSL), Transport Layer Security (TLS) | Used to provide secure communication over the internet |
| Transmission Control Protocol (TCP) | Ensures packets are transmitted reliably and in the correct order |
