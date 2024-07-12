# Course 2: 

## Module 1: Security Domains

### Learning Objectives

    Recognize and explain the focus of CISSP's eight security domains.
    Identify and define the primary threats, risks, and vulnerabilities to business operations.
    Describe the threats, risks, and vulnerabilities that entry-level security analysts are most focused on.
    Determine how threats, risks, and vulnerabilities impact business operations.
    Identify the steps of risk management.

### Security domains cybersecurity analysts need to know

#### Domain one: Security and risk management

All organizations must develop their security posture. Security posture is an organization’s ability to manage its defense of critical assets and data and react to change. Elements of the security and risk management domain that impact an organization's security posture include:

    Security goals and objectives
    Risk mitigation processes
    Compliance
    Business continuity plans
    Legal regulations
    Professional and organizational ethics

Information security, or InfoSec, is also related to this domain and refers to a set of processes established to secure information. An organization may use playbooks and implement training as a part of their security and risk management program, based on their needs and perceived risk. There are many InfoSec design processes, such as:

    Incident response
    Vulnerability management
    Application security
    Cloud security
    Infrastructure security

As an example, a security team may need to alter how personally identifiable information (PII) is treated in order to adhere to the European Union's General Data Protection Regulation (GDPR).

#### Domain two: Asset security

Asset security involves managing the cybersecurity processes of organizational assets, including the storage, maintenance, retention, and destruction of physical and virtual data. Because the loss or theft of assets can expose an organization and increase the level of risk, keeping track of assets and the data they hold is essential. Conducting a security impact analysis, establishing a recovery plan, and managing data exposure will depend on the level of risk associated with each asset. Security analysts may need to store, maintain, and retain data by creating backups to ensure they are able to restore the environment if a security incident places the organization’s data at risk.

#### Domain three: Security architecture and engineering	

This domain focuses on managing data security. Ensuring effective tools, systems, and processes are in place helps protect an organization’s assets and data. Security architects and engineers create these processes.

One important aspect of this domain is the concept of shared responsibility. Shared responsibility means all individuals involved take an active role in lowering risk during the design of a security system. Additional design principles related to this domain, which are discussed later in the program, include:

    Threat modeling
    Least privilege
    Defense in depth
    Fail securely
    Separation of duties
    Keep it simple
    Zero trust
    Trust but verify

An example of managing data is the use of a security information and event management (SIEM) tool to monitor for flags related to unusual login or user activity that could indicate a threat actor is attempting to access private data.

#### Domain four: Communication and network security

This domain focuses on managing and securing physical networks and wireless communications. This includes on-site, remote, and cloud communications. 

Organizations with remote, hybrid, and on-site work environments must ensure data remains secure, but managing external connections to make certain that remote workers are securely accessing an organization’s networks is a challenge. Designing network security controls—such as restricted network access—can help protect users and ensure an organization’s network remains secure when employees travel or work outside of the main office. 

#### Domain five: Identity and access management

The identity and access management (IAM) domain focuses on keeping data secure. It does this by ensuring user identities are trusted and authenticated and that access to physical and logical assets is authorized. This helps prevent unauthorized users, while allowing authorized users to perform their tasks.

Essentially, IAM uses what is referred to as the principle of least privilege, which is the concept of granting only the minimal access and authorization required to complete a task. As an example, a cybersecurity analyst might be asked to ensure that customer service representatives can only view the private data of a customer, such as their phone number, while working to resolve the customer's issue; then remove access when the customer's issue is resolved.

#### Domain six: Security assessment and testing 

The security assessment and testing domain focuses on identifying and mitigating risks, threats, and vulnerabilities. Security assessments help organizations determine whether their internal systems are secure or at risk. Organizations might employ penetration testers, often referred to as “pen testers,” to find vulnerabilities that could be exploited by a threat actor. 

This domain suggests that organizations conduct security control testing, as well as collect and analyze data. Additionally, it emphasizes the importance of conducting security audits to monitor for and reduce the probability of a data breach. To contribute to these types of tasks, cybersecurity professionals may be tasked with auditing user permissions to validate that users have the correct levels of access to internal systems.

#### Domain seven: Security operations 

The security operations domain focuses on the investigation of a potential data breach and the implementation of preventative measures after a security incident has occurred. This includes using strategies, processes, and tools such as:

    Training and awareness
    Reporting and documentation
    Intrusion detection and prevention
    SIEM tools   
    Log management
    Incident management
    Playbooks
    Post-breach forensics
    Reflecting on lessons learned

The cybersecurity professionals involved in this domain work as a team to manage, prevent, and investigate threats, risks, and vulnerabilities. These individuals are trained to handle active attacks, such as large amounts of data being accessed from an organization's internal network, outside of normal working hours. Once a threat is identified, the team works diligently to keep private data and information safe from threat actors.  

#### Domain eight: Software development security

The software development security domain is focused on using secure programming practices and guidelines to create secure applications. Having secure applications helps deliver secure and reliable services, which helps protect organizations and their users.

Security must be incorporated into each element of the software development life cycle, from design and development to testing and release. To achieve security, the software development process must have security in mind at each step. Security cannot be an afterthought.

Performing application security tests can help ensure vulnerabilities are identified and mitigated accordingly. Having a system in place to test the programming conventions, software executables, and security measures embedded in the software is necessary. Having quality assurance and pen tester professionals ensure the software has met security and performance standards is also an essential part of the software development process. For example, an entry-level analyst working for a pharmaceutical company might be asked to make sure encryption is properly configured for a new medical device that will store private patient data. 

### Manage common threats, risks, and vulnerabilities

#### Risk management

A primary goal of organizations is to protect assets. An asset is an item perceived as having value to an organization. Assets can be digital or physical. Examples of digital assets include the personal information of employees, clients, or vendors, such as: 

    Social Security Numbers (SSNs), or unique national identification numbers assigned to individuals 
    Dates of birth
    Bank account numbers
    Mailing addresses

Examples of physical assets include:

    Payment kiosks
    Servers
    Desktop computers
    Office spaces

Some common strategies used to manage risks include:

    Acceptance: Accepting a risk to avoid disrupting business continuity
    Avoidance: Creating a plan to avoid the risk altogether
    Transference: Transferring risk to a third party to manage
    Mitigation: Lessening the impact of a known risk

Additionally, organizations implement risk management processes based on widely accepted frameworks to help protect digital and physical assets from various threats, risks, and vulnerabilities. Examples of frameworks commonly used in the cybersecurity industry include the National Institute of Standards and Technology Risk Management Framework (NIST RMF) and Health Information Trust Alliance (HITRUST).

#### Today’s most common threats, risks, and vulnerabilities

##### Threats

A threat is any circumstance or event that can negatively impact assets. As an entry-level security analyst, your job is to help defend the organization’s assets from inside and outside threats. Therefore, understanding common types of threats is important to an analyst’s daily work. As a reminder, common threats include:

    Insider threats: Staff members or vendors abuse their authorized access to obtain data that may harm an organization.

    Advanced persistent threats (APTs): A threat actor maintains unauthorized access to a system for an extended period of time.

##### Risks

A risk is anything that can impact the confidentiality, integrity, or availability of an asset. A basic formula for determining the level of risk is that risk equals the likelihood of a threat. One way to think about this is that a risk is being late to work and threats are traffic, an accident, a flat tire, etc. 

There are different factors that can affect the likelihood of a risk to an organization’s assets, including:

    External risk: Anything outside the organization that has the potential to harm organizational assets, such as threat actors attempting to gain access to private information

    Internal risk: A current or former employee, vendor, or trusted partner who poses a security risk

    Legacy systems: Old systems that might not be accounted for or updated, but can still impact assets, such as workstations or old mainframe systems. For example, an organization might have an old vending machine that takes credit card payments or a workstation that is still connected to the legacy accounting system.

    Multiparty risk: Outsourcing work to third-party vendors can give them access to intellectual property, such as trade secrets, software designs, and inventions.

    Software compliance/licensing: Software that is not updated or in compliance, or patches that are not installed in a timely manner

There are many resources, such as the NIST, that provide lists of cybersecurity risks. Additionally, the Open Web Application Security Project (OWASP) publishes a standard awareness document about the top 10 most critical security risks
 to web applications, which is updated regularly. 

##### Vulnerabilities

A vulnerability is a weakness that can be exploited by a threat. Therefore, organizations need to regularly inspect for vulnerabilities within their systems. Some vulnerabilities include:

    ProxyLogon: A pre-authenticated vulnerability that affects the Microsoft Exchange server. This means a threat actor can complete a user authentication process to deploy malicious code from a remote location.

    ZeroLogon: A vulnerability in Microsoft’s Netlogon authentication protocol. An authentication protocol is a way to verify a person's identity. Netlogon is a service that ensures a user’s identity before allowing access to a website's location.

    Log4Shell: Allows attackers to run Java code on someone else’s computer or leak sensitive information. It does this by enabling a remote attacker to take control of devices connected to the internet and run malicious code.

    PetitPotam: Affects Windows New Technology Local Area Network (LAN) Manager (NTLM). It is a theft technique that allows a LAN-based attacker to initiate an authentication request.

    Security logging and monitoring failures: Insufficient logging and monitoring capabilities that result in attackers exploiting vulnerabilities without the organization knowing it

    Server-side request forgery: Allows attackers to manipulate a server-side application into accessing and updating backend resources. It can also allow threat actors to steal data.

As an entry-level security analyst, you might work in vulnerability management, which is monitoring a system to identify and mitigate vulnerabilities. Although patches and updates may exist, if they are not applied, intrusions can still occur. For this reason, constant monitoring is important. The sooner an organization identifies a vulnerability and addresses it by patching it or updating their systems, the sooner it can be mitigated, reducing the organization’s exposure to the vulnerability. 

To learn more about the vulnerabilities explained in this section of the reading, as well as other vulnerabilities, explore the NIST National Vulnerability Database and CISA Known Exploited Vulnerabilities Catalog.

### Glossary terms from module 1 

**Assess**: The fifth step of the NIST RMF that means to determine if established controls are implemented correctly

**Authorize**: The sixth step of the NIST RMF that refers to being accountable for the security and privacy risks that may exist in an organization

**Business continuity**: An organization's ability to maintain their everyday productivity by establishing risk disaster recovery plans

**Categorize**: The second step of the NIST RMF that is used to develop risk management processes and tasks

**External threat**: Anything outside the organization that has the potential to harm organizational assets

**Implement**: The fourth step of the NIST RMF that means to implement security and privacy plans for an organization

**Internal threat**: A current or former employee, external vendor, or trusted partner who poses a security risk

**Monitor**: The seventh step of the NIST RMF that means be aware of how systems are operating

**Prepare**: The first step of the NIST RMF related to activities that are necessary to manage security and privacy risks before a breach occurs

**Ransomware**: A malicious attack where threat actors encrypt an organization’s data and demand payment to restore access 

**Risk**: Anything that can impact the confidentiality, integrity, or availability of an asset

**Risk mitigation**: The process of having the right procedures and rules in place to quickly reduce the impact of a risk like a breach

**Security posture**: An organization’s ability to manage its defense of critical assets and data and react to change

**Select**: The third step of the NIST RMF that means to choose, customize, and capture documentation of the controls that protect an organization

**Shared responsibility**: The idea that all individuals within an organization take an active role in lowering risk and maintaining both physical and virtual security

**Social engineering**: A manipulation technique that exploits human error to gain private information, access, or valuables 

**Vulnerability**: A weakness that can be exploited by a threat

## Module 2: Security framework and controls

### Learning Objectives

    Define and describe the purpose of security frameworks and controls.
    Describe the CIA triad.
    Explain the National Institute of Standards and Technology (NIST) frameworks.
    Identify security principles.
    Examine how businesses use security frameworks and controls to protect business operations.
    Define security audits.
    Explore common elements of internal security audits.

### The relationship between frameworks and controls

#### Frameworks and controls

`Security frameworks` are `guidelines` used for building plans to help mitigate risk and threats to data and privacy. Frameworks support organizations’ ability to adhere to compliance laws and regulations. For example, the healthcare industry uses frameworks to comply with the United States’ Health Insurance Portability and Accountability Act (HIPAA), which requires that medical professionals keep patient information safe. 

`Security controls` are `safeguards` designed to reduce specific security risks. Security controls are the measures organizations use to lower risk and threats to data and privacy. For example, a control that can be used alongside frameworks to ensure a hospital remains compliant with HIPAA is requiring that patients use multi-factor authentication (MFA) to access their medical records. Using a measure like MFA to validate someone’s identity is one way to help mitigate potential risks and threats to private data.

#### Specific frameworks and controls

##### Cyber Threat Framework (CTF)

According to the Office of the Director of National Intelligence, the CTF was developed by the U.S. government to provide “a common language for describing and communicating information about cyber threat activity.” By providing a common language to communicate information about threat activity, the CTF helps cybersecurity professionals analyze and share information more efficiently. This allows organizations to improve their response to the constantly evolving cybersecurity landscape and threat actors' many tactics and techniques.

##### International Organization for Standardization/International Electrotechnical Commission (ISO/IEC) 27001

An internationally recognized and used framework is ISO/IEC 27001. The ISO 27000 family of standards enables organizations of all sectors and sizes to manage the security of assets, such as financial information, intellectual property, employee data, and information entrusted to third parties. This framework outlines requirements for an information security management system, best practices, and controls that support an organization’s ability to manage risks. Although the ISO/IEC 27001 framework does not require the use of specific controls, it does provide a collection of controls that organizations can use to improve their security posture. 
Controls

Controls are used alongside frameworks to reduce the possibility and impact of a security threat, risk, or vulnerability. Controls can be physical, technical, and administrative and are typically used to prevent, detect, or correct security issues.

Examples of physical controls:

    Gates, fences, and locks

    Security guards

    Closed-circuit television (CCTV), surveillance cameras, and motion detectors

    Access cards or badges to enter office spaces

Examples of technical controls:

    Firewalls

    MFA

    Antivirus software

Examples of administrative controls:

    Separation of duties

    Authorization

    Asset classification

To learn more about controls, particularly those used to protect health-related assets from a variety of threat types, review the U.S. Department of Health and Human Services’ Physical Access Control presentation. 

### Use the CIA triad to protect organizations

#### The CIA triad for analysts

The CIA triad is a model that helps inform how organizations consider risk when setting up systems and security policies. It is made up of three elements that cybersecurity analysts and organizations work toward upholding: confidentiality, integrity, and availability. Maintaining an acceptable level of risk and ensuring systems and policies are designed with these elements in mind helps establish a successful security posture, which refers to an organization’s ability to manage its defense of critical assets and data and react to change. 

`Confidentiality` is the idea that only authorized users can access specific assets or data. In an organization, confidentiality can be enhanced through the implementation of design principles, such as the principle of least privilege. The principle of least privilege limits users' access to only the information they need to complete work-related tasks. Limiting access is one way of maintaining the confidentiality and security of private data. 

`Integrity` is the idea that the data is verifiably correct, authentic, and reliable. Having protocols in place to verify the authenticity of data is essential. One way to verify data integrity is through cryptography, which is used to transform data so unauthorized parties cannot read or tamper with it (NIST, 2022). Another example of how an organization might implement integrity is by enabling encryption, which is the process of converting data from a readable format to an encoded format. Encryption can be used to prevent access and ensure data, such as messages on an organization's internal chat platform, cannot be tampered with.  

`Availability` is the idea that data is accessible to those who are authorized to use it. When a system adheres to both availability and confidentiality principles, data can be used when needed. In the workplace, this could mean that the organization allows remote employees to access its internal network to perform their jobs. It’s worth noting that access to data on the internal network is still limited, depending on what type of access employees need to do their jobs. If, for example, an employee works in the organization’s accounting department, they might need access to corporate accounts but not data related to ongoing development projects. 

### NIST frameworks

5 Functions: Identify, Protect, Detect, Respond, Recover

`Identify` is related to the management of cybersecurity risk and its effect on an organization's people and assets. 

`Protect` is the strategy used to protect an organization through the implementation of policies, procedures, training, and tools that help mitigate cybersecurity threats. 

`Detect` means identifying potential security incidents and improving monitoring capabilities to increase the speed and efficiency of detections.


`Respond` means making sure that the proper procedures are used to contain, neutralize,
and analyze security incidents, and implement improvements to the security process. 

`Recover` is the process of returning affected systems back to normal operation. 

### OWASP security principles (Open Web Application Security Project)

1. Minimize the attack surface area

Attack surface refers to all the potential vulnerabilities a threat actor could exploit.

2. Least privilege 

Users have the least amount of access required to perform their everyday tasks.

3. Defense in depth

Organizations should have varying security controls that mitigate risks and threats.

4. Separation of duties

Critical actions should rely on multiple people, each of whom follow the principle of least privilege. 

5. Keep security simple

Avoid unnecessarily complicated solutions. Complexity makes security difficult. 

6. Fix security issues correctly

When security incidents occur, identify the root cause, contain the impact, identify vulnerabilities, and conduct tests to ensure that remediation is successful.

7. Establish secure defaults

This principle means that the optimal security state of an application is also its default state for users; it should take extra work to make the application insecure. 

8. Fail securely

Fail securely means that when a control fails or stops, it should do so by defaulting to its most secure option. For example, when a firewall fails it should simply close all connections and block all new ones, rather than start accepting everything.

9. Don’t trust services

Many organizations work with third-party partners. These outside partners often have different security policies than the organization does. And the organization shouldn’t explicitly trust that their partners’ systems are secure. For example, if a third-party vendor tracks reward points for airline customers, the airline should ensure that the balance is accurate before sharing that information with their customers.

10. Avoid security by obscurity

The security of an application should not rely on keeping the source code secret. Its security should rely upon many other factors, including reasonable password policies, defense in depth, business transaction limits, solid network architecture, and fraud and audit controls.

### Security Audits

#### Definition

A security audit is a review of an organization's security controls, policies, and procedures against a set of expectations. Audits are independent reviews that evaluate whether an organization is meeting internal and external criteria. Internal criteria include outlined policies, procedures, and best practices. External criteria include regulatory compliance, laws, and federal regulations. 

Additionally, a security audit can be used to assess an organization's established security controls. As a reminder, security controls are safeguards designed to reduce specific security risks. 

Audits help ensure that security checks are made (i.e., daily monitoring of security information and event management dashboards), to identify threats, risks, and vulnerabilities. This helps maintain an organization’s security posture. And, if there are security issues, a remediation process must be in place.

#### Goals and objectives of an audit

The goal of an audit is to ensure an organization's information technology (IT) practices are meeting industry and organizational standards. The objective is to identify and address areas of remediation and growth. Audits provide direction and clarity by identifying what the current failures are and developing a plan to correct them. 

Security audits must be performed to safeguard data and avoid penalties and fines from governmental agencies. The frequency of audits is dependent on local laws and federal compliance regulations.

#### Factors that affect audits

Factors that determine the types of audits an organization implements include: 

    Industry type

    Organization size

    Ties to the applicable government regulations

    A business’s geographical location

    A business decision to adhere to a specific regulatory compliance

#### The role of frameworks and controls in audits

Along with compliance, it’s important to mention the role of frameworks and controls in security audits. Frameworks such as the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF) and the international standard for information security (ISO 27000) series are designed to help organizations prepare for regulatory compliance security audits. By adhering to these and other relevant frameworks, organizations can save time when conducting external and internal audits. Additionally, frameworks, when used alongside controls, can support organizations’ ability to align with regulatory compliance requirements and standards.  

There are three main categories of controls to review during an audit, which are administrative and/or managerial, technical, and physical controls. 

#### Audit checklist

1. Identify the scope of the audit

    The audit should:

        List assets that will be assessed (e.g., firewalls are configured correctly, PII is secure, physical assets are locked, etc.) 

        Note how the audit will help the organization achieve its desired goals

        Indicate how often an audit should be performed

        Include an evaluation of organizational policies, protocols, and procedures to make sure they are working as intended and being implemented by employees

2. Complete a risk assessment

A risk assessment is used to evaluate identified organizational risks related to budget, controls, internal processes, and external standards (i.e., regulations).

3. Conduct the audit

When conducting an internal audit, you will assess the security of the identified assets listed in the audit scope.

4. Create a mitigation plan

A mitigation plan is a strategy established to lower the level of risk and potential costs, penalties, or other issues that can negatively affect the organization’s security posture. 

5. Communicate results to stakeholders

The end result of this process is providing a detailed report of findings, suggested improvements needed to lower the organization's level of risk, and compliance regulations and standards the organization needs to adhere to. 

### Glossary terms from module 2

**Asset**: An item perceived as having value to an organization

**Attack vectors**: The pathways attackers use to penetrate security defenses

**Authentication**: The process of verifying who someone is

**Authorization**: The concept of granting access to specific resources in a system

**Availability**: The idea that data is accessible to those who are authorized to access it

**Biometrics**: The unique physical characteristics that can be used to verify a person’s identity

**Confidentiality**: The idea that only authorized users can access specific assets or data

**Confidentiality, integrity, availability (CIA) triad**: A model that helps inform how organizations consider risk when setting up systems and security policies

**Detect**: A NIST core function related to identifying potential security incidents and improving monitoring capabilities to increase the speed and efficiency of detections

**Encryption**: The process of converting data from a readable format to an encoded format

**Identify**: A NIST core function related to management of cybersecurity risk and its effect on an organization’s people and assets 

**Integrity**: The idea that the data is correct, authentic, and reliable

**National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF)**: A voluntary framework that consists of standards, guidelines, and best practices to manage cybersecurity risk 

**National Institute of Standards and Technology (NIST) Special Publication (S.P.) 800-53**: A unified framework for protecting the security of information systems within the U.S. federal government 

**Open Web Application Security Project/Open Worldwide Application Security Project (OWASP)**: A non-profit organization focused on improving software security

**Protect**: A NIST core function used to protect an organization through the implementation of policies, procedures, training, and tools that help mitigate cybersecurity threats

**Recover**: A NIST core function related to returning affected systems back to normal operation

**Respond**: A NIST core function related to making sure that the proper procedures are used to contain, neutralize, and analyze security incidents, and implement improvements to the security process

**Risk**: Anything that can impact the confidentiality, integrity, or availability of an asset

**Security audit**: A review of an organization's security controls, policies, and procedures against a set of expectations

**Security controls**: Safeguards designed to reduce specific security risks 

**Security frameworks**: Guidelines used for building plans to help mitigate risk and threats to data and privacy

**Security posture**: An organization’s ability to manage its defense of critical assets and data and react to change

**Threat**: Any circumstance or event that can negatively impact assets


## Module 3: Introduction to cybersecurity tools

### Learning Objectives

    Identify and define commonly used Security Information and Event Management (SIEM) tools.
    Describe how SIEM tools are used to protect business operations.
    Explain how entry-level security analysts use SIEM dashboards.

### 






## Module 4: Use playbooks to respond to incidents

### Learning Objectives

    Define and describe the purpose of a playbook.
    Use a playbook to respond to identified threats, risks, or vulnerabilities.

### 






