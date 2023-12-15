# Introduction to the Internet
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

## How the Internet Works
- The core of the internet is a global network of interconnected routers
- When data is sent over the internet, it is broken up into small packets
- The router examines the packet and forwards it to the next router in the path towards its destination
- The process continues until the packet reaches its final destination
- IP and TCP ensure packets are sent and received correctly

## Building Applications with TCP/IP
- TCP/IP is the underlying communication protocol used by most internet-based applications and services
- Provides a reliable, ordered, and error-checked delivery of data between applications running on different devices
- Key concepts to understand:

| Term | Description |
|--|--|
| Port | Used to identify the application or service running on a device. Each application or service is assigned a unique port number, allowing data to be sent to the correct destination. |
| Socket | A combination of IP address and a port number, representing a specific endpoint for communication. Used to establish connections between devices and transfer data between applications. |
| Connection | Established between two sockets when two devices want to communicate with each other. During the connection establishment process, the devices negotiate various parameters such as the maximum segment size and window size, which determine how data will be transmitted over the connection. |
| Data transfer | Once a connection is established, data can be transferred between applications running on each device. Data is typically transmitted in segments, with each segment containing a sequence number and other metadata to ensure reliable delivery. |

## Securing Internet Communication with SSL/TLS
- SSL and TLS are protocols used to encrypt data being transmitted over the internet
- Commonly used to provide secure connections for applications such as web browsers, email clients, and file transfer programs
- Few key concepts to understand:

| Term | Description |
|--|--|
| Certificate | SSL/TLS certificates are used to establish trust about the client and server. They contain information about the identity of the server and are signed by a trusted third party (a Certificate Authority) to verify their authenticity. |
| Handshake | During the SSL/TLS handshake process, the client and server exchange information to negotiate the encryption algorithm and other parameters for the secure connection. |
| Encryption | Once the secure connection is established, data is encrypted using the agreed-upon algorithm and other parameters for the secure connection. |
- Ensure that your application is designed to use SSL/TLS when transmitting sensitive data such as login credentials, payment information, and other personal data
- Also ensure you obtain and maintain valid SSL/TLS certificates for your servers


## Glossary
| Term | Description |
|--|--|
| 5G | The latest generation of mobile network technology, offering faster speeds, lower latency, and greater capacity than previous generations. It is expected to enable new use cases and applications, such as autonomous vehicles and remote surgery. |
| Artificial Intelligence (AI) | AI technologies such as machine learning and natural language processing are already being used to power a wide range of applications and services, from voice assistants to fraud detection. It is expected to enable new use cases and transform industries such as healthcare, finance, and education. |
| Blockchain | A distributed ledger technology that enables secure, decentralized transactions. It is being used to power a wide range of applications, from cryptocurrency to supply chain management. |
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
