

# Networking Notes

## OSI Model (7 Layers)

It breaks down the process of sending data into 7 distinct layers.

### Layer 7 - Application

Purpose:  Where the user interacts (web browser, a game client,...).
Examples:         

**Web Browsing:** **HTTP** / **HTTPS**

* **File Transfer:** **FTP** / **SFTP** (used by applications like FileZilla to upload files to a server)

* **Email:** **SMTP** (sending mail), **IMAP** or **POP3** (retrieving mail used by Outlook or Gmail).

* **Network Utilities:** **DNS** (translating "google.com" to an IP address), 

* **DHCP** (automatically assigning IP addresses to devices joining a network).

### Layer 6 - Presentation

Purpose:  Translates, encrypts, or compresses data ( JSON, SSL/TLS,...).
Examples:

- **Data Formatting & Serialization:** **JSON**, **XML**, or **YAML** (how API data is structured so different programming languages can read it).

- **Encryption & Security:** **SSL/TLS** (the encryption layer that turns standard HTTP into secure HTTPS).

- **Compression:** **JPEG**, **PNG** (for images), or **MP4** (for video), which compress raw data into standardized formats before transmission.

### Layer 5 - Session

Purpose:  Manages the connection between the two devices (opening, managing, and closing communication sessions).
Examples:

- **Authentication & Authorization:** Protocols like **RADIUS** which manage user logins and keep track of who is allowed to do what during a session.

- **Remote Connections:** **RPC** (Remote Procedure Call) and **SQL Session** management, which keep a database connection open while an application runs queries.

### Layer 4 - Transport

Purpose:  Chooses *how* to send data (TCP or UDP) and manages flow control.
Examples:

- **TCP (Transmission Control Protocol):** Connection-oriented and reliable. Used for **Web browsing (HTTP)**, **Email**,etc.. . If a packet goes missing, TCP pauses and asks for a re-send.

- **UDP (User Datagram Protocol):** Connectionless and fast. Used for **Live video streaming**, **Online gaming**, and **VOIP (voice calls)**. It doesn't check if packets arrive; it just keeps sending them to maintain real-time speed.

### Layer 3 - Network

Purpose:  Routing data packets across different networks. It handles logical addressing (where things are globally).
Examples:

* **Core Protocols:** **IPv4** and **IPv6** (the unique IP addresses assigned to your device and servers worldwide).

* **RIP** (the algorithms routers use to find the fastest path across the internet).

* **Hardware:** **Routers** and **Layer 3 Switches** operate here, reading IP headers to send packets to the correct destination network.

### Layer 2 - Data Link

Purpose:  Handles physical addressing (**MAC addresses**).
Examples:

- **Local Networking:** **Ethernet** (IEEE 802.3) for wired local networks, and **Wi-Fi** (IEEE 802.11) for wireless local networks.

- **Addressing:** **MAC Addresses** (the permanent, burned-in hardware address unique to your network interface card).

- **Hardware:** **Network Switches** (Layer 2) and **Access Points**, which look at MAC addresses to send data to the specific device in the office or home.

### Layer 1 - Physical

Purpose:  The actual hardware—cables, radio waves, bits of 1s and 0s.
Examples:

- **Cabling:** **Ethernet cables** (copper twisted pair), **Fiber-optic cables** (pulses of light), and **Coaxial cables** (used by cable internet).

- **Wireless Mediums:** **Radio waves** (used by Wi-Fi, Bluetooth, and 5G/LTE cellular networks).

- **Hardware Components:** **Network Interface Cards (NICs)**, **Hubs**, **Repeaters**, and **RJ45 connectors**.

## TCP/IP Model (4 Layers)

The OSI model is great for theory, but the **TCP/IP model** is how the actual internet is built. It condenses the world into 4 practical layers:

### Application Layer (Combines OSI Layers 5, 6, and 7)

Purpose:  
Examples:


