# Course 6: Sound the Alarm: Detection and Response

## Module 1: Introduction to detection and incident response 

### Roles in response

the National Institute of Standards and Technology (NIST) Incident Response Lifecycle (a framework for incident response)

    Preparation
    Detection and Analysis
    Containment, Eradication, and Recovery
    Post-incident activity

#### Command, control, and communication

A computer security incident response team (CSIRT) is a specialized group of security professionals that are trained in incident management and response. During incident response, teams can encounter a variety of different challenges. For incident response to be effective and efficient, there must be clear command, control, and communication of the situation to achieve the desired goal. 

    Command refers to having the appropriate leadership and direction to oversee the response.

    Control refers to the ability to manage technical aspects during incident response, like coordinating resources and assigning tasks.

    Communication refers to the ability to keep stakeholders informed.

Establishing a CSIRT organizational structure with clear and distinctive roles aids in achieving an effective and efficient response.

#### Roles in CSIRTs 

CSIRTs are organization dependent, so they can vary in their structure and operation. Structurally, they can exist as a separate, dedicated team or as a task force that meets when necessary. CSIRTs involve both nonsecurity and security professionals. Nonsecurity professionals are often consulted to offer their expertise on the incident. These professionals can be from external departments, such as human resources, public relations, management, IT, legal, and others. Security professionals involved in a CSIRT typically include three key security related roles: 

1. Security analyst

2. Technical lead

3. Incident coordinator

##### Security analyst

The job of the security analyst is to continuously monitor an environment for any security threats. This includes: 

    Analyzing and triaging alerts
    Performing root-cause investigations
    Escalating or resolving alerts 

If a critical threat is identified, then analysts escalate it to the appropriate team lead, such as the technical lead.

##### Technical lead

The job of the technical lead is to manage all of the technical aspects of the incident response process, such as applying software patches or updates. They do this by first determining the root cause of the incident. Then, they create and implement the strategies for containing, eradicating, and recovering from the incident. Technical leads often collaborate with other teams to ensure their incident response priorities align with business priorities, such as reducing disruptions for customers or returning to normal operations. 

##### Incident coordinator

Responding to an incident also requires cross-collaboration with nonsecurity professionals. CSIRTs will often consult with and leverage the expertise of members from external departments. The job of the incident coordinator is to coordinate with the relevant departments during a security incident. By doing so, the lines of communication are open and clear, and all personnel are made aware of the incident status. Incident coordinators can also be found in other teams, like the SOC. 

##### Other roles

Depending on the organization, many other roles can be found in a CSIRT, including a dedicated communications lead, a legal lead, a planning lead, and more. 

Note: Teams, roles, responsibilities, and organizational structures can differ for each company. For example, some different job titles for incident coordinator include incident commander and incident manager.

#### Security operations center

A security operations center (SOC) is an organizational unit dedicated to monitoring networks, systems, and devices for security threats or attacks. Structurally, a SOC (usually pronounced "sock") often exists as its own separate unit or within a CSIRT. You may be familiar with the term blue team, which refers to the security professionals who are responsible for defending against all security threats and attacks at an organization. A SOC is involved in various types of blue team activities, such as network monitoring, analysis, and response to incidents. 

#### SOC organization

A SOC is composed of SOC analysts, SOC leads, and SOC managers. Each role has its own respective responsibilities. SOC analysts are grouped into three different tiers. 

##### Tier 1 SOC analyst

The first tier is composed of the least experienced SOC analysts who are known as level 1s (L1s). They are responsible for:

    Monitoring, reviewing, and prioritizing alerts based on criticality or severity
    Creating and closing alerts using ticketing systems
    Escalating alert tickets to Tier 2 or Tier 3

##### Tier 2 SOC analyst

The second tier comprises the more experienced SOC analysts, or level 2s (L2s). They are responsible for: 

    Receiving escalated tickets from L1 and conducting deeper investigations
    Configuring and refining security tools
    Reporting to the SOC Lead

##### Tier 3 SOC lead

The third tier of a SOC is composed of the SOC leads, or level 3s (L3s). These highly experienced professionals are responsible for:

    Managing the operations of their team
    Exploring methods of detection by performing advanced detection techniques, such as malware and forensics analysis
    Reporting to the SOC manager

##### SOC manager 

The SOC manager is at the top of the pyramid and is responsible for: 

    Hiring, training, and evaluating the SOC team members
    Creating performance metrics and managing the performance of the SOC team
    Developing reports related to incidents, compliance, and auditing
    Communicating findings to stakeholders such as executive management   

##### Other roles

SOCs can also contain other specialized roles such as: 

    Forensic investigators: Forensic investigators are commonly L2s and L3s who collect, preserve, and analyze digital evidence related to security incidents to determine what happened.

    Threat hunters: Threat hunters are typically L3s who work to detect, analyze, and defend against new and advanced cybersecurity threats using threat intelligence.

Note: Just like CSIRTs, the organizational structure of a SOC can differ depending on the organization. 

### Overview of detection tools

Detection tools work similarly to home security systems. Whereas home security systems monitor and protect homes against intrusion, cybersecurity detection tools help organizations protect their networks and systems against unwanted and unauthorized access. For organizations to protect their systems from security threats or attacks, they must be made aware when there is any indication of an intrusion. Detection tools make security professionals aware of the activity happening on a network or a system. The tools do this by continuously monitoring networks and systems for any suspicious activity. Once something unusual or suspicious is detected, the tool triggers an alert that notifies the security professional to investigate and stop the possible intrusion. 

#### Overview of IDS tools

An intrusion detection system (IDS) is an application that monitors system activity and alerts on possible intrusions. An IDS provides continuous monitoring of network events to help protect against security threats or attacks. The goal of an IDS is to detect potential malicious activity and generate an alert once such activity is detected. An IDS does not stop or prevent the activity. Instead, security professionals will investigate the alert and act to stop it, if necessary. 

For example, an IDS can send out an alert when it identifies a suspicious user login, such as an unknown IP address logging into an application or a device at an unusual time. But, an IDS will not stop or prevent any further actions, like blocking the suspicious user login. 

Examples of IDS tools include Zeek, Suricata, Snort®, and Sagan. 

##### Detection categories

As a security analyst, you will investigate alerts that an IDS generates. There are four types of detection categories you should be familiar with:

    A true positive is an alert that correctly detects the presence of an attack.

    A true negative is a state where there is no detection of malicious activity. This is when no malicious activity exists and no alert is triggered. 

    A false positive is an alert that incorrectly detects the presence of a threat. This is when an IDS identifies an activity as malicious, but it isn't. False positives are an inconvenience for security teams because they spend time and resources investigating an illegitimate alert. 

    A false negative is a state where the presence of a threat is not detected. This is when malicious activity happens but an IDS fails to detect it. False negatives are dangerous because security teams are left unaware of legitimate attacks that they can be vulnerable to. 

#### Overview of IPS tools

An intrusion prevention system (IPS) is an application that monitors system activity for intrusive activity and takes action to stop the activity. An IPS works similarly to an IDS. But, IPS monitors system activity to detect and alert on intrusions, and it also takes action to prevent the activity and minimize its effects. For example, an IPS can send an alert and modify an access control list on a router to block specific traffic on a server.

Note: Many IDS tools can also operate as an IPS. Tools like Suricata, Snort, and Sagan have both IDS and IPS capabilities.

#### Overview of EDR tools 

Endpoint detection and response (EDR) is an application that monitors an endpoint for malicious activity. EDR tools are installed on endpoints. Remember that an endpoint is any device connected on a network. Examples include end-user devices, like computers, phones, tablets, and more.

EDR tools monitor, record, and analyze endpoint system activity to identify, alert, and respond to suspicious activity. Unlike IDS or IPS tools, EDRs collect endpoint activity data `and perform behavioral analysis` to identify threat patterns happening on an endpoint. Behavioral analysis uses the power of machine learning and artificial intelligence to analyze system behavior to identify malicious or unusual activity. EDR tools also use automation to stop attacks without the manual intervention of security professionals. For example, if an EDR detects an unusual process starting up on a user’s workstation that normally is not used, it can automatically block the process from running.

Tools like Open EDR®, Bitdefender™ Endpoint Detection and Response, and FortiEDR™ are examples of EDR tools.

Note: Security information and event management (SIEM) tools also have detection capabilities, which you'll explore later.

### Overview of SIEM technology

#### SIEM advantages

SIEM tools collect and manage security-relevant data that can be used during investigations. This is important because SIEM tools provide awareness about the activity that occurs between devices on a network. The information SIEM tools provide can help security teams quickly investigate and respond to security incidents. SIEM tools have many advantages that can help security teams effectively respond to and manage incidents. Some of the advantages are:

    Access to event data: SIEM tools provide access to the event and activity data that happens on a network, including real-time activity. Networks can be connected to hundreds of different systems and devices. SIEM tools have the ability to ingest all of this data so that it can be accessed.

    Monitoring, detecting, and alerting: SIEM tools continuously monitor systems and networks in real-time. They then analyze the collected data using detection rules to detect malicious activity. If an activity matches the rule, an alert is generated and sent out for security teams to assess.

    Log storage: SIEM tools can act as a system for data retention, which can provide access to historical data. Data can be kept or deleted after a period depending on an organization's requirements. 

#### The SIEM process

1. Collect and aggregate data

SIEM tools require data for them to be effectively used. During the first step, the SIEM collects event data from various sources like firewalls, servers, routers, and more. This data, also known as logs, contains event details like timestamps, IP addresses, and more. Logs are a record of events that occur within an organization’s systems. After all of this log data is collected, it gets aggregated in one location. Aggregation refers to the process of consolidating log data into a centralized place. Through collection and aggregation, SIEM tools eliminate the need for manually reviewing and analyzing event data by accessing individual data sources. Instead, all event data is accessible in one location—the SIEM. Parsing can occur during the first step of the SIEM process when data is collected and aggregated. Parsing maps data according to their fields and their corresponding values.

2. Normalize data 

SIEM tools collect data from many different sources. This data must be transformed into a single format so that it can be easily processed by the SIEM. However, each data source is different and data can be formatted in many different ways. For example, a firewall log can be formatted differently than a server log. Collected event data should go through the process of normalization. Normalization converts data into a standard, structured format that is easily searchable. 

3. Analyze data

After log data has been collected, aggregated, and normalized, the SIEM must do something useful with all of the data to enable security teams to investigate threats. During this final step in the process, SIEM tools analyze the data. Analysis can be done with some type of detection logic such as a set of rules and conditions. SIEM tools then apply these rules to the data, and if any of the log activity matches a rule, alerts are sent out to cybersecurity teams.

Note: A part of the analysis process includes correlation. Correlation involves the comparison of multiple log events to identify common patterns that indicate potential security threats.

#### SIEM tools 

There are many SIEM tools. The following are some SIEM tools commonly used in the cybersecurity industry:

    AlienVault® OSSIM™
    Chronicle
    Elastic
    Exabeam
    IBM QRadar® Security Intelligence Platform
    LogRhythm
    Splunk

### Glossary terms from module 1

**Computer security incident response teams (CSIRT)**: A specialized group of security professionals that are trained in incident management and response 

**Documentation**: Any form of recorded content that is used for a specific purpose 

**Endpoint detection and response (EDR)**: An application that monitors an endpoint for malicious activity

**Event**: An observable occurrence on a network, system, or device

**False negative**: A state where the presence of a threat is not detected

**False positive**: An alert that incorrectly detects the presence of a threat

**Incident**: An occurrence that actually or imminently jeopardizes, without lawful authority, the confidentiality, integrity, or availability of information or an information system; or constitutes a violation or imminent threat of violation of law, security policies, security procedures, or acceptable use policies

**Incident handler’s journal**: A form of documentation used in incident response

**Incident response plan**: A document that outlines the procedures to take in each step of incident response

**Intrusion detection system (IDS)**: An application that monitors system activity and alerts on possible intrusions

**Intrusion prevention system (IPS)**: An application that monitors system activity for intrusive activity and takes action to stop the activity

**National Institute of Standards and Technology (NIST) Incident Response Lifecycle**: A framework for incident response consisting of four phases: Preparation; Detection and Analysis; Containment, Eradication, and Recovery; and Post-incident activity

**Playbook**: A manual that provides details about any operational action

**Security information and event management (SIEM)**: An application that collects and analyzes log data to monitor critical activities in an organization 

**Security operations center (SOC)**: An organizational unit dedicated to monitoring networks, systems, and devices for security threats or attacks

**Security orchestration, automation, and response (SOAR)**: A collection of applications, tools, and workflows that uses automation to respond to security events

**True negative**: A state where there is no detection of malicious activity

**True positive**: An alert that correctly detects the presence of an attack  


## Module 2: Network monitoring and analysis

### Maintain awareness with network monitoring

Network communication can be noisy! Events like sending an email, streaming a video, or visiting a website all produce network communications in the form of network traffic and network data. As a reminder, network traffic is the amount of data that moves across a network. It can also include the type of data that is transferred, such as HTTP. Network data is the data that's transmitted between devices on a network.

Network monitoring is essential in maintaining situational awareness of any activity on a network. By collecting and analyzing network traffic, organizations can detect suspicious network activity. But before networks can be monitored, you must know exactly what to monitor. In this reading, you'll learn more about the importance of network monitoring, ways to monitor your network, and network monitoring tools.

Networks connect devices, and devices then communicate and exchange data using network protocols. Network communications provide information about connections such as source and destination IP addresses, amount of data transferred, date and time, and more. This information can be valuable for security professionals when developing a baseline of normal or expected behavior. 

A baseline is a reference point that’s used for comparison. You've probably encountered or used baselines at some point. For example, a grocery amount for a personal budget is an example of a baseline that can be used to help identify any patterns or changes in spending habits. In security, baselines help establish a standard of expected or normal behavior for systems, devices, and networks. Essentially, by knowing the baseline of normal network behavior, you'll be better able to identify abnormal network behavior.

#### Monitor your network

Once you’ve determined a baseline, you can monitor a network to identify any deviations from that baseline. Monitoring involves examining network components to detect unusual activities, such as large and unusual data transfers. Here are examples of network components that can be monitored to detect malicious activity:

##### Flow analysis

Flow refers to the movement of network communications and includes information related to packets, protocols, and ports. Packets can travel to ports, which receive and transmit communications. Ports are often, but not always, associated with network protocols. For example, port 443 is commonly used by HTTPS which is a protocol that provides website traffic encryption.

However, malicious actors can use protocols and ports that are not commonly associated to maintain communications between the compromised system and their own machine. These communications are what’s known as command and control (C2), which are the techniques used by malicious actors to maintain communications with compromised systems.

For example, malicious actors can use HTTPS protocol over port 8088 as opposed to its commonly associated port 443 to communicate with compromised systems. Organizations must know which ports should be open and approved for connections, and watch out for any mismatches between ports and their associated protocols.

##### Packet payload information

Network packets contain components related to the transmission of the packet. This includes details like source and destination IP address, and the packet payload information, which is the actual data that’s transmitted. Often, this data is encrypted and requires decryption for it to be readable. Organizations can monitor the payload information of packets to uncover unusual activity, such as sensitive data transmitting outside of the network, which could indicate a possible data exfiltration attack.

##### Temporal patterns

Network packets contain information relating to time. This information is useful in understanding time patterns. For example, a company operating in North America experiences bulk traffic flows between 9 a.m. to 5 p.m., which is the baseline of normal network activity. If large volumes of traffic are suddenly outside of the normal hours of network activity, then this is considered off baseline and should be investigated.

Through network monitoring, organizations can promptly detect network intrusions and work to prevent them from happening by securing network components.

#### Lateral movement

In network security, lateral movement is the process by which attackers spread from an entry point to the rest of the network. There are many methods by which they can achieve this. For instance, an attack could start with malware on an employee's desktop computer. From there, the attacker attempts to move laterally to infect other computers on the network, to infect internal servers, and so on until they reach their final target.

#### Protect your network

In this program, you’ve learned about security operations centers (SOC) and their role in monitoring systems against security threats and attacks. Organizations may deploy a network operations center (NOC), which is an organizational unit that monitors the performance of a network and responds to any network disruption, such as a network outage. While a SOC is focused on maintaining the security of an organization through detection and response, a NOC is responsible for maintaining network performance, availability, and uptime. 

Security analysts monitor networks to identify any signs of potential security incidents known as indicators of compromise (IoC) and  protect networks from threats or attacks. To do this, they must understand the environment that network communications travel through so that they can identify deviations in network traffic. 

#### Network monitoring tools

Network monitoring can be automated or performed manually. Some common network monitoring tools can include: 

Intrusion detection systems (IDS) monitor system activity and alert on possible intrusions. An IDS will detect and alert on the deviations you’ve configured it to detect. Most commonly, IDS tools will monitor the content of packet payload to detect patterns associated with threats such as malware or phishing attempts.

Network protocol analyzers, also known as packet sniffers, are tools designed to capture and analyze data traffic within a network. They can be used to analyze network communications manually in detail. Examples include tools such as tcpdump and Wireshark, which can be used by security professionals to record network communications through packet captures. Packet captures can then be investigated to identify potentially malicious activity.

### Learn more about packet captures

The role of security analysts involves monitoring and analyzing network traffic flows. One way to do this is by generating packet captures and then analyzing the captured traffic to identify unusual activity on a network.

#### Packets

Previously in the program, you learned that a data packet is a basic unit of information that travels from one device to another within a network. Detecting network intrusions begins at the packet level. That's because packets form the basis of information exchange over a network. Each time you perform an activity on the internet—like visiting a website—packets are sent and received between your computer and the website’s server. These packets are what help transmit information through a network. For example, when uploading an image to a website, the data gets broken up into multiple packets, which then get routed to the intended destination and reassembled upon delivery. 

In cybersecurity, packets provide valuable information that helps add context to events during investigations. Understanding the transfer of information through packets will not only help you develop insight on network activity, it will also help you identify abnormalities and better defend networks from attacks.

Packets contain three components: the header, the payload, and the footer. Here’s a description of each of these components.

##### Header

Packets begin with the most essential component: the header. Packets can have several headers depending on the protocols used such as an Ethernet header, an IP header, a TCP header, and more. Headers provide information that’s used to route packets to their destination. This includes information about the source and destination IP addresses, packet length, protocol, packet identification numbers, and more. 

Here is an IPv4 header with the information it provides:
```
Version    IHL   TOS   Total Length
Identification   Flags   Fragment Offset
TTL   Protocol   Header Checksum
Source address
Destination address
Options
```
##### Payload

The payload component directly follows the header and contains the actual data being delivered. Think back to the example of uploading an image to a website; the payload of this packet would be the image itself.

##### Footer

The footer, also known as the trailer, is located at the end of a packet. The Ethernet protocol uses footers to provide error-checking information to determine if data has been corrupted. In addition, Ethernet network packets that are analyzed might not display footer information due to network configurations.

Note: Most protocols, such as the Internet Protocol (IP), do not use footers. 

#### Network protocol analyzers

Network protocol analyzers (packet sniffers) are tools designed to capture and analyze data traffic within a network. Examples of network protocol analyzers include tcpdump, Wireshark, and TShark. 

Beyond their use in security as an investigative tool used to monitor networks and identify suspicious activity, network protocol analyzers can be used to collect network statistics, such as bandwidth or speed, and troubleshoot network performance issues, like slowdowns. 

Network protocol analyzers can also be used for malicious purposes. For example, malicious actors can use network protocol analyzers to capture packets containing sensitive data, such as account login information.

Here’s a network diagram illustrating how packets get transmitted from a sender to the receiver. A network protocol analyzer is placed in the middle of the communications to capture the data packets that travel over the wire.

#### How network protocol analyzers work

Network protocol analyzers use both software and hardware capabilities to capture network traffic and display it for security analysts to examine and analyze. Here’s how:

1. First, packets must be collected from the network via the Network Interface Card (NIC), which is hardware that connects computers to a network, like a router. NICs receive and transmit network traffic, but by default they only listen to network traffic that’s addressed to them. To capture all network traffic that is sent over the network, a NIC must be switched to a mode that has access to all visible network data packets. In wireless interfaces this is often referred to as monitoring mode, and in other systems it may be called promiscuous mode. This mode enables the NIC to have access to all visible network data packets, but it won’t help analysts access all packets across a network. A network protocol analyzer must be positioned in an appropriate network segment to access all traffic between different hosts. 

2. The network protocol analyzer collects the network traffic in raw binary format. Binary format consists of 0s and 1s and is not as easy for humans to interpret. The network protocol analyzer takes the binary and converts it so that it’s displayed in a human-readable format, so analysts can easily read and understand the information.  

#### Capturing packets

Packet sniffing is the practice of capturing and inspecting data packets across a network. A packet capture (p-cap) is a file containing data packets intercepted from an interface or network. Packet captures can be viewed and further analyzed using network protocol analyzers. For example, you can filter packet captures to only display information that's most relevant to your investigation, such as packets sent from a specific IP address.

Note: Using network protocol analyzers to intercept and examine private network communications without permission is considered illegal in many places.

P-cap files can come in many formats depending on the packet capture library that’s used. Each format has different uses and network tools may use or support specific packet capture file formats by default. You should be familiar with the following libraries and formats:


1. Libpcap is a packet capture library designed to be used by Unix-like systems, like Linux and MacOS®. Tools like tcpdump use Libpcap as the default packet capture file format. 

2. WinPcap is an open-source packet capture library designed for devices running Windows operating systems. It’s considered an older file format and isn’t predominantly used.

3. Npcap is a library designed by the port scanning tool Nmap that is commonly used in Windows operating systems.

4. PCAPng is a modern file format that can simultaneously capture packets and store data. Its ability to do both explains the “ng,” which stands for “next generation.”


### Investigate packet details

#### Internet Protocol (IP)

Packets form the foundation of data exchange over a network, which means that detection begins at the packet level. The Internet Protocol (IP) includes a set of standards used for routing and addressing data packets as they travel between devices on a network. IP operates as the foundation for all communications over the internet.

IP ensures that packets reach their destinations. There are two versions of IP that you will find in use today: IPv4 and IPv6. Both versions use different headers to structure packet information. 

##### IPv4

IPv4 is the most commonly used version of IP. There are thirteen fields in the header:

`Version`: This field indicates the IP version. For an IPv4 header, IPv4 is used. 

`Internet Header Length (IHL)`: This field specifies the length of the IPv4 header including any Options.

`Type of Service (ToS)`: This field provides information about packet priority for delivery.

`Total Length`: This field specifies the total length of the entire IP packet including the header and the data.

`Identification`: Packets that are too large to send are fragmented into smaller pieces. This field specifies a unique identifier for fragments of an original IP packet so that they can be reassembled once they reach their destination.

`Flags`: This field provides information about packet fragmentation including whether the original packet has been fragmented and if there are more fragments in transit.

`Fragment Offset`: This field is used to identify the correct sequence of fragments.

`Time to Live (TTL)`: This field limits how long a packet can be circulated in a network, preventing packets from being forwarded by routers indefinitely.

`Protocol`: This field specifies the protocol used for the data portion of the packet.

`Header Checksum`: This field specifies a checksum value which is used for error-checking the header.

`Source Address`: This field specifies the source address of the sender.

`Destination Address`: This field specifies the destination address of the receiver.

`Options`: This field is optional and can be used to apply security options to a packet.


##### IPv6

IPv6 adoption has been increasing because of its large address space. There are eight fields in the header:

`Version`: This field indicates the IP version. For an IPv6 header, IPv6 is used.

`Traffic Class`: This field is similar to the IPv4 Type of Service field. The Traffic Class field provides information about the packet's priority or class to help with packet delivery.

`Flow Label`: This field identifies the packets of a flow. A flow is the sequence of packets sent from a specific source. 

`Payload Length`: This field specifies the length of the data portion of the packet.

`Next Header`: This field indicates the type of header that follows the IPv6 header such as TCP.

`Hop Limit`: This field is similar to the IPv4 Time to Live field. The Hop Limit limits how long a packet can travel in a network before being discarded.

`Source Address`: This field specifies the source address of the sender.

`Destination Address`: This field specifies the destination address of the receiver.

#### Wireshark

Wireshark is an open-source network protocol analyzer. It uses a graphical user interface (GUI), which makes it easier to visualize network communications for packet analysis purposes. Wireshark has many features to explore that are beyond the scope of this course. You'll focus on how to use basic filtering to isolate network packets so that you can find what you need.

##### Display filters

Wireshark's display filters let you apply filters to packet capture files. This is helpful when you are inspecting packet captures with large volumes of information. Display filters will help you find specific information that's most relevant to your investigation. You can filter packets based on information such as protocols, IP addresses, ports, and virtually any other property found in a packet. Here, you'll focus on display filtering syntax and filtering for protocols, IP addresses, and ports.

##### Comparison operators

You can use different comparison operators to locate specific header fields and values. Comparison operators can be expressed using either abbreviations or symbols. For example, this filter using the == equal symbol in this filter ip.src == 8.8.8.8 is identical to using the eq abbreviation in this filter ip.src eq 8.8.8.8.

Pro tip: You can combine comparison operators with Boolean logical operators like and and or to create complex display filters. Parentheses can also be used to group expressions and to prioritize search terms.

##### Contains operator

The contains operator is used to filter packets that contain an exact match of a string of text. Here is an example of a filter that displays all HTTP streams that match the keyword "moved". 

##### Matches operator

The matches operator is used to filter packets based on the regular expression (regex) that's specified. Regular expression is a sequence of characters that forms a pattern. You'll explore more about regular expressions later in this program. 

#### Filter toolbar

You can apply filters to a packet capture using Wireshark's filter toolbar. In this example, dns is the applied filter, which means Wireshark will only display packets containing the DNS protocol.

Pro tip: Wireshark uses different colors to represent protocols. You can customize colors and create your own filters.

##### Filter for protocols

Protocol filtering is one of the simplest ways you can use display filters. You can simply enter the name of the protocol to filter. For example, to filter for DNS packets simply type dns in the filter toolbar. Here is a list of some protocols you can filter for:

    dns
    http
    ftp
    ssh
    arp
    telnet
    icmp

##### Filter for an IP address

You can use display filters to locate packets with a specific IP address. 

For example, if you would like to filter packets that contain a specific IP address use ip.addr, followed by a space, the equal == comparison operator, and the IP address. Here is an example of a display filter that filters for the IP address 172.21.224.2:

ip.addr == 172.21.224.2

To filter for packets originating from a specific source IP address, you can use the ip.src filter. Here is an example that looks for the 10.10.10.10 source IP address:

ip.src == 10.10.10.10

To filter for packets delivered to a specific destination IP address, you can use the ip.dst filter. Here is an example that searches for the 4.4.4.4 destination IP address:

ip.dst == 4.4.4.4

Filter for a MAC address
You can also filter packets according to the Media Access Control (MAC) address. As a refresher, a MAC address is a unique alphanumeric identifier that is assigned to each physical device on a network.

Here's an example:

eth.addr == 00:70:f4:23:18:c4

##### Filter for ports

Port filtering is used to filter packets based on port numbers. This is helpful when you want to isolate specific types of traffic. DNS traffic uses TCP or UDP port 53 so this will list traffic related to DNS queries and responses only.

For example, if you would like to filter for a UDP port:

udp.port == 53

Likewise, you can filter for TCP ports as well:

tcp.port == 25

#### Follow streams

Wireshark provides a feature that lets you filter for packets specific to a protocol and view streams. A stream or conversation is the exchange of data between devices using a protocol. Wireshark reassembles the data that was transferred in the stream in a way that's simple to read.

Following a protocol stream is useful when trying to understand the details of a conversation. For example, you can examine the details of an HTTP conversation to view the content of the exchanged request and response messages.

### Overview of tcpdump

#### Concepts: 

A network protocol analyzer (packet sniffer) is a tool designed to capture and analyze data traffic within a network.

Packet sniffing is the practice of capturing and inspecting data packets across a network. 

#### tcpdump

Tcpdump is a command-line network protocol analyzer. Recall that a command-line interface (CLI) is a text-based user interface that uses commands to interact with the computer. 

Tcpdump is used to capture network traffic. This traffic can be saved to a packet capture (p-cap), which is a file containing data packets intercepted from an interface or network. The p-cap file can be  accessed, analyzed, or shared at a later time. Analysts use tcpdump for a variety of reasons, from troubleshooting network issues to identifying malicious activity. Tcpdump comes pre-installed in many Linux distributions and can also be installed on other Unix-based operating systems such as macOS®. 

Note: It's common for network traffic to be encrypted, which means data is encoded and unreadable. Inspecting the network packets might require decrypting the data using the appropriate private keys. 

#### Capturing packets with tcpdump

Previously in this program, you learned that a Linux root user (or superuser) has elevated privileges to modify the system. You also learned that the sudo command temporarily grants elevated permissions to specific users in Linux. Like many other packet sniffing tools, you’ll need to have administrator-level privileges to capture network traffic using tcpdump. This means you will need to either be logged in as the root user or have the ability to use the sudo command. Here is a breakdown of the tcpdump syntax for capturing packets:

sudo tcpdump [-i interface] [option(s)] [expression(s)]

    The sudo tcpdump command begins running tcpdump using elevated permissions as sudo. 

    The -i parameter specifies the network interface to capture network traffic. You must specify a network interface to capture from to begin capturing packets. For example, if you specify -i any you’ll sniff traffic from all network interfaces on the system. 

    The option(s) are optional and provide you with the ability to alter the execution of the command. The expression(s) are a way to further filter network traffic packets so that you can isolate network traffic. You’ll learn more about option(s) and expression(s) in the next section.

Note: Before you can begin capturing network traffic, you must identify which network interface you'll want to use to capture packets from. You can use the -D flag to list the network interfaces available on a system.

#### Options

With tcpdump, you can apply options, also known as flags, to the end of commands to filter network traffic. Short options are abbreviated and represented by a hyphen and a single character like -i. Long options are spelled out using a double hyphen like --interface. Tcpdump has over fifty options that you can explore using the manual page. Here, you’ll examine a couple of essential tcpdump options including how to write and read packet capture files. 

Note: Options are case sensitive. For example, a lowercase -w is a separate option with a different use than the option with an uppercase -W.

Note: tcpdump options that are written using short options can be written with or without a space between the option and its value. For example, sudo tcpdump -i any -c 3 and sudo tcpdump -iany -c3 are equivalent commands.

##### -w

Using the -w flag, you can write or save the sniffed network packets to a packet capture file instead of just printing it out in the terminal. This is very useful because you can refer to this saved file for later analysis. In this command, tcpdump is capturing network traffic from all network interfaces and saving it to a packet capture file named packetcapture.pcap:

```
sudo tcpdump -i any -w packetcapture.pcap
```

##### -r

Using the -r flag, you can read a packet capture file by specifying the file name as a parameter. Here is an example of a tcpdump command that reads a file called packetcapture.pcap:

```
sudo tcpdump -r packetcapture.pcap
```

##### -v

As you’ve learned, packets contain a lot of information. By default, tcpdump will not print out all of a packet's information. This option, which stands for verbose, lets you control how much packet information you want tcpdump to print out.

There are three levels of verbosity you can use depending on how much packet information you want tcpdump to print out. The levels are -v, -vv, and -vvv. The level of verbosity increases with each added v. The verbose option can be helpful if you’re looking for packet information like the details of a packet’s IP header fields. Here’s an example of a tcpdump command that reads the packetcapture.pcap file with verbosity:

```
sudo tcpdump -r packetcapture.pcap -v
```

##### -c

The -c option stands for count. This option lets you control how many packets tcpdump will capture. For example, specifying -c 1 will only print out one single packet, whereas -c 10 prints out 10 packets. This example is telling tcpdump to only capture the first three packets it sniffs from any network interface:

```
sudo tcpdump -i any -c 3
```

##### -n  

By default, tcpdump will perform name resolution. This means that tcpdump automatically converts IP addresses to names. It will also resolve ports to commonly associated services that use these ports. This can be problematic because tcpdump isn’t always accurate in name resolution. For example, tcpdump can capture traffic from port 80 and automatically translates port 80 to HTTP in the output. However, this is misleading because port 80 isn’t always going to be using HTTP; it could be using a different protocol.

Additionally, name resolution uses what’s known as a reverse DNS lookup. A reverse DNS lookup is a query that looks for the domain name associated with an IP address. If you perform a reverse DNS lookup on an attacker’s system, they might be alerted that you are investigating them through their DNS records.

Using the -n flag disables this automatic mapping of numbers to names and is considered to be best practice when sniffing or analyzing traffic. Using -n will not resolve hostnames, whereas -nn will not resolve both hostnames or ports. Here’s an example of a tcpdump command that reads the packetcapture.pcap file with verbosity and disables name resolution:
```
sudo tcpdump -r packetcapture.pcap -v -n
```

Pro tip: You can combine options together. For example, -v and -n can be combined as -vn. But, if an option accepts a parameter right after it like -c 1 or -r capture.pcap then you can’t combine other options to it.

#### Expressions

Using filter expressions in tcpdump commands is also optional, but knowing how and when to use filter expressions can be helpful during packet analysis. There are many ways to use filter expressions. 

If you want to specifically search for network traffic by protocol, you can use filter expressions to isolate network packets. For example, you can filter to find only IPv6 traffic using the filter expression ip6.

You can also use boolean operators like and, or, or not to further filter network traffic for specific IP addresses, ports, and more. The example below reads the packetcapture.pcap file and combines two expressions ip and port 80 using the and boolean operator:

```
sudo tcpdump -r packetcapture.pcap -n 'ip and port 80'
```

Pro tip: You can use single or double quotes to ensure that tcpdump executes all of the expressions. You can also use parentheses to group and prioritize different expressions. Grouping expressions is helpful for complex or lengthy commands. For example, the command ip and (port 80 or port 443) tells tcpdump to prioritize executing the filters enclosed in the parentheses before filtering for IPv4.

#### Interpreting output

Once you run a command to capture packets, tcpdump will print the output of the command as the sniffed packets. In the output, tcpdump prints one line of text for each packet with each line beginning with a timestamp. Here’s an example of a command and output for a single TCP packet: 

```
sudo tcpdump -i any -v -c 1
```

This command tells tcpdump to capture packets on -i any network interface. The option -v prints out the packet with detailed information and the option -c 1 prints out only one packet. 

```
<Timestamp> IP <Source IP>.<Source port> > <Destination IP>.<Destination port>: Flags [P.],seq 120:176, ack 1, win 501, options [nop, nop, TS val 4106659748 ecr 2979487360], length 144
```

Timestamp: The output begins with the timestamp, which starts with hours, minutes, seconds, and fractions of a second. 

Source IP: The packet’s origin is provided by its source IP address.

Source port: This port number is where the packet originated.

Destination IP: The destination IP address is where the packet is being transmitted to.

Destination port: This port number is where the packet is being transmitted to.

The remaining output contains details of the TCP connection including flags and sequence number. The options information is additional packet information that the  -v option has provided.






## Module 3: Incident investigation and response












## Module 4: Network traffic and logs using IDS and SIEM tools














