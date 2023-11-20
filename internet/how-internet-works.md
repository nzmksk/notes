# Introduction to the Internet
- Developed in 1960s by the US Department of Defense
- To create a decentralized communication network that could withstand a **nuclear attack**

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


## Glossary
| Term | Description |
|--|--|
| Domain Name | A human-readable name that is used to identify a website, such as google.com |
| Domain Name System (DNS) | Responsible for translating domain names into IP addresses |
| Hypertext Transfer Protocol (HTTP) | Used to transfer data between a client (e.g. web browser) and a server (e.g. website) |
| Hypertext Transfer Protocol Secure (HTTPS) | An encrypted version of HTTP using SSL/TLS encryption |
| IP Address | A unique identifier assigned to each device on a network, used to route data to the correct destination |
| Internet | A network of networks |
| Internet Protocol (IP) | Responsible for routing packets to their correct destination |
| Network | A group of computers or other devices connected to each other |
| Packet | A small unit of data that is transmitted over the internet |
| Router | Responsible for directing traffic between different devices and systems |
| Secure Sockets Layer (SSL), Transport Layer Security (TLS) | Used to provide secure communication over the internet |
| Transmission Control Protocol (TCP) | Ensures packets are transmitted reliably and in the correct order |
