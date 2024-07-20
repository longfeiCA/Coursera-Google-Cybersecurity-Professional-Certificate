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








## Module 3: Incident investigation and response












## Module 4: Network traffic and logs using IDS and SIEM tools














