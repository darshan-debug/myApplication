# Project: Design and Implementation of GBN & SR - Transport Layer Protocols

This project details the design and implementation of the **Go-Back-N (GBN)** and **Selective Repeat (SR)** protocols.  
Built with a **Java-based GUI**, the application provides a visual comparison of how these transport layer protocols ensure **Reliable Data Transfer (RDT)** over an unreliable network.

---

## 📚 Key Concepts and Features

The core of this project demonstrates fundamental concepts of computer networking:

- **Reliable Data Transfer (RDT):**  
  The protocols guarantee the integrity, delivery, and correct ordering of data segments.

- **Checksums:**  
  Used for error detection within data packets.

- **Sequence Numbers:**  
  Essential for maintaining packet order and identifying duplicate packets during re-transmission.

- **Pipelining:**  
  Enhances network utilization by allowing the sender to transmit multiple packets without waiting for an acknowledgment for each one,  
  a significant improvement over the inefficient *stop-and-wait* approach.

- **Acknowledgments (ACK):**  
  The receiver's feedback mechanism to confirm successful packet reception.  
  - **GBN:** Uses *cumulative ACKs* (an ACK for packet **T** implies all packets up to **T** have been received correctly).

---

## 🚀 Go-Back-N (GBN) Protocol

The GUI application simulates the **GBN protocol** with:
- **Sender-side window size:** 5  
- **Receiver-side window size:** 1  

➡️ This means the sender can have up to **five unacknowledged packets** in transit at any given time.  
If a timeout occurs for any packet, the sender **re-transmits all unacknowledged packets** currently in its window,  
showcasing the classic **"Go-Back-N" behavior**.

---

## 💻 Core Technology Stack

This project is built on **Java**, leveraging several key libraries and frameworks to implement the protocol simulation and the graphical user interface:

- **Java Swing:**  
  The entire application's GUI (frames, buttons, labels, text areas) is built using the Swing library.  
  This allows for a visual representation of the GBN protocol, making it easier to understand packet flow and state changes.

- **Java Networking:**  
  The core communication between sender and receiver is handled by Java's networking capabilities.  
  - `ServerSocket` and `Socket` classes are used to establish a **TCP connection** for reliable, ordered data transfer.

- **I/O Streams:**  
  - `DataInputStream` and `DataOutputStream` are used to send/receive primitive data types (like integers for packet sequence numbers).  
  - This ensures correct serialization and deserialization of data packets.

---

### 🧑‍💻 Developed By:

<b>DARSHAN KUMAR</b><br>
 Software Engineer<br>
linkedin: [connect with me, here!](https://www.linkedin.com/in/darshan-k-489226201/)

<br><br><br><br>
---
---