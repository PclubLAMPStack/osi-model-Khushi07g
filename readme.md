# 7 layers of the OSI Model

The OSI (Open Systems Interconnection) model is a conceptual framework that provides a standardized way to describe how computer network protocols communicate with each other.
The OSI model divides the network communication process into seven distinct layers, each of which is responsible for specific functions and services.

1) `Physical layer` - The Physical layer is the first layer in the OSI model and deals with the physical aspects of network communication. Its main responsibility is to transmit raw data bits over the network medium and includes equipments involved in data transfer such as cables, connectors, and network interface cards.

   The Physical layer is responsible for encoding data into a specific sequence of electrical or optical signals that can be transmitted over the network medium. It also specifies the signaling and data transfer rates used by the network.

   This layer handles other physical aspects of network communication, such as voltage levels, timing of signals, and synchronization between devices. It also detects physical errors that may occur during transmission, such as cable breaks, signal attenuation, and interference.

2) `Data link layer` - This layer is responsible for the error-free transfer of data frames. It does this by breaking up the data into smaller units called frames, and adding header and trailer information to each frame. This information includes source and destination addresses, sequence numbers, and error detection codes which helps to ensure that the data is transmitted accurately and received without errors.

   The Data Link layer also handles error detection and correction. It checks for errors in the received data and uses error detection codes to identify any errors that may have occurred during transmission. If errors are detected, the Data Link layer will request that the sender retransmit the data to ensure that it is received correctly.

   The Data Link layer also handles flow control. This helps to regulate the flow of data between the sender and receiver to prevent overload and congestion, and it can use techniques such as buffering and rate limiting to control the flow of data.

   It includes two sublayers: 

   - Logical Link Control (LLC)- The LLC sublayer provides a common interface to the network layer.
   - Media Access Control (MAC)- The MAC sublayer controls access to the physical network medium.

3) `Network layer` - The network layer is responsible for facilitating data transfer between two different networks.

   The Network layer receives data from the upper layers and encapsulates it into packets that include source and destination IP addresses. It then determines the best path for the packet to reach its destination, using routing protocols such as OSPF or BGP. The Network layer may also perform fragmentation of packets if necessary, to ensure that they can be transmitted across networks with different Maximum Transmission Unit (MTU) sizes.

   In addition to routing, the Network layer also provides congestion control. It can also perform traffic shaping to control the rate of traffic flowing between different network segments.

4) `Transport layer` - The fourth layer and the heart of the OSI model is the Transport layer, which is responsible for end-to-end communication between applications on different devices. Its main function is to provide reliable and transparent transfer of data between the source and destination devices.

   The Transport layer receives data from the upper layers and breaks it into smaller units called segments. These segments are numbered and sequenced to ensure that they are transmitted and received in the correct order. The Transport layer also provides error detection and correction to ensure that data is transmitted accurately.

   The Transport layer uses two main protocols: 

   - Transmission Control Protocol (TCP):
       - Connection-oriented protocol that establishes a reliable connection between the source and destination devices before transmitting data.
       - Provides flow control, congestion control, and error recovery mechanisms to ensure that data is transmitted accurately and efficiently.
    
   - User Datagram Protocol (UDP):
       - Connectionless protocol that does not establish a connection before transmitting data. 
       - Provides faster transmission speeds and lower latency than TCP, as there is no connection setup or teardown overhead.
       - Used for applications that require faster transmission speeds and do not require reliability or error detection and correction, such as online gaming or real-time streaming.


5) `Session layer` - The fifth layer of the OSI model is the Session layer whose main function is to establish, maintain, and terminate communication sessions between applications.

   he Session layer provides services such as session establishment, synchronization, and termination, as well as managing data exchange between applications. It also provides checkpointing and recovery mechanisms to ensure that data exchange can be resumed in the event of a network failure.

   The Session layer also handles security and authentication functions, such as encrypting and decrypting data, and verifying the identities of communicating devices.

6) `Presentation layer` - The sixth layer of the OSI model is the Presentation layer, which is responsible for translating, formatting, and presenting data in a way that can be understood by the application layer. Its main function is to provide a common representation of data exchanged between applications, regardless of the different data formats and protocols used by the communicating devices.

   The Presentation layer provides several services to accomplish this, including:

   - Data translation: The Presentation layer can translate data into a common format that can be understood by the application layer. This can involve converting data between different character sets, data types, or encoding schemes.
   - Data compression: The Presentation layer can compress data to reduce the amount of data that needs to be transmitted over the network to improve network performance. 
   - Data encryption and decryption: The Presentation layer can encrypt data to provide secure transmission of data over the network.
   - Data formatting: The Presentation layer can format data in a way that is compatible with the receiving application. This can involve adding or removing headers, footers, or other formatting information.

7) `Application layer` - The seventh layer of the OSI model is the Application layer, which is the layer that is closest to the end user. It is responsible for providing services that are used by end-user applications, such as email, web browsers, and file transfer programs. The Application layer acts as the interface between the user and the network, providing a user-friendly way to access network resources.

   The Application layer provides several services to accomplish this, including:

   - Network virtual terminal: The Application layer provides a virtual terminal that allows the user to access resources on the network. This can include accessing remote files, running remote applications, or accessing network printers.
   - File transfer and management: The Application layer provides services that allow users to transfer files between devices and manage files on the network.
   - Email services: The Application layer provides email services that allow users to send and receive email messages over the network. 
   - Web services: The Application layer provides web services that allow users to access web pages and other resources on the Internet. 

In conclusion, the OSI model is a conceptual framework that describes how network protocols and communications should be structured and organized. The model consists of seven layers, each with a specific function and set of services that work together to ensure that data is transmitted efficiently and reliably across a network.



