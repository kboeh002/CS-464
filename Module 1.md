# Module 1: Course Overview and Introduction
## Table of Contents
##### 1. Overview
##### 1.A. Assignments
##### 1.1 Scope and Sequence of Online Course
##### 1.2 Introduction to Network Security
###### 1.2.1 Computer Security vs Network Security
###### 1.2.2 Definitions and Concepts of Security
###### 1.2.3 The OSI Security Architecture
###### 1.2.4 Security Attacks
###### 1.2.5 Security Services
###### 1.2.6 Security Mechanisms
###### 1.2.7 A Model for Network Security
###### 1.2.8 Learning Check
##### 1.S. Summary

*Note: Anything that has a linked [#] is from an external source outside of the notes.*

## 1.2 Introduction to Network Security
### 1.2.1 Computer Security vs Network Security
* **Computer/Information Security:** the collection of tools designed to protect data and thwart hackers
* **Network/Internet Security:** the collection of tools to protect data and communcation between interconnected networks
* ***i*nternet:** (lowercase i) refers to any interconnected *collecton* of networks
* ***I*nternet:** (uppercase I) a *specific example* of internet
    * Network security measures are needed to protect data during transmission
* **Computer Virus:** one of the most publicized types of attacks on information systems; arrive over the internet or from physically on an optical disk loaded into a computer
* Security Violations eg. man-in-the-middle, spoofing, repudiation
### 1.2.2 Definitions and Concepts of Security
* **Computer Security:** "The protection afforded to an automated information system in order to attain the applicable objectives of preserving the integrity, availability, and confidentiality of information system resources (includes hardware, software, firmware, information/data, and telecommunications)." ([National Insititutes for Standards and Technology](http://www.nist.gov/))
* **CIA Triad:** the key objectives of Computer/Network Security
1. *Confidentiality:*
    * **Data Confidentiality:** Assures that private/confidential info is not available to unauthorized individuals
    * **Privacy:** Assures that individuals control/influence what info related to them may be collected and stored and by/to whom it may be disclosed to
2. *Integrity:*
    * **Data Integrity:** Assures that info and programs are changed only in a specified and authorized manner
    * **System Integrity:** Assures that a system performs its intended function in an unimpared manner, free from deliberate or inadvertent unauthorized manipulation of the system
3. *Availability:*
    * **Availability:** Assures that systems work promptly and service is not denied to authorized users
* **Authenticity:** Verfies that users are who they say they are and that each input arriving at the system came from a trusted source
* **Accountability:** Generates the requirement for actions of the entitiy to be traced uniquely to that entity in order to trace a security breach to a responsible party
### 1.2.3 The OSI Security Architecture
* **International Telecommunication Union-Telecomunication Standardization Sector (ITU-T):** agency sponsored by the United Nations that develops standards
    * they reccomend X.800 Security Architecture for OSI
* **Open Systems Interconnection (OSI):** (model) is a conceptual model that provides a common basis for the coordination of ISO standards of development [[1](https://en.wikipedia.org/wiki/OSI_model)]; is a framework that describes networking or telecommunications systems in layers [[2](https://www.networkworld.com/article/3239677/the-osi-model-explained-and-how-to-easily-remember-its-7-layers.html)]
* **OSI Network Architecture:** defines a systematic approach for defining the requirements for security of an organization and characterizes the approaches to satisfying those requirements
    * Focuses on security attacks, mechanisms and services:
        * **Security Attack:** any action that compromises the security of information owned by an organization
        * **Security Mechanism:** a process (or device incorperating the process) that is designed to detect, prevent, or recover from a security attack
        * **Security Service:** a processing or communication service that enhances the security of the data processing systems and the information transfers of an organization; intended to counter security attacks making use of $\ge$ 1 security mechanisms
### 1.2.4 Security Attacks
#### Security Attacks
* **Internet Engineering Task Force (IETF):** a standards organization for the internet and is responsible for the technical standards that make up the internet [[3](https://en.wikipedia.org/wiki/Internet_Engineering_Task_Force)]; defines standard operating internet protocols (eg. TCP, IP) [[4](https://www.techtarget.com/whatis/definition/IETF-Internet-Engineering-Task-Force)]
* **Internet Architecture Board (IAB):** "provides long range technical direction for Internet development, ensuring the Internet continues to grow and evolve as a platform and continues to grow and evolve as a platform for global communication and innovation" [[5](https://www.iab.org/)] and strives to...
    * "Ensure that the Internet is a trusted medium of communication that provides a solid technical foundation for privacy and security, especially in light of pervasive surveillance" [[5](https://www.iab.org/)]
    * "Establish the technical direction for an Internet that will enable billions more people to connect, support the vision for an Internet of Things, and allow mobile networks to flourish, while keeping the core capabilities that have been a foundation of the Internet’s success" [[5](https://www.iab.org/)]
    * "Promote the technical evolution of an open Internet without special controls, especially those which hinder trust in the network." [[5](https://www.iab.org/)] 
* **Requests For Comment (RFC):** a formal document from the IETF that contains specifications and organizational notes about topics related to the internet and computer networking (eg. routing, addressing, and transport technologies) [[6](https://www.techtarget.com/whatis/definition/Request-for-Comments-RFC#:~:text=Robert%20Sheldon-,What%20is%20a%20Request%20for%20Comments%20(RFC)%3F,routing%2C%20addressing%20and%20transport%20technologies.)]
* **Security Attack:** "An assault on a system security that derives from an *intelligent* threat." (definition from RFC no. 2828 from IETF and IAB)
    * **Intelligent Threat:**  an intelligent act that is a deliberate attempt (especially in the sense of a method or technique) to evade security services and to violate the security policy of a system (definition from RFC no. 2828 from IETF and IAB)
    * X.800 and RFC 2828 classify security attacks as either passive or active
#### Passive Attacks
* **Passive Attack:** attempts to learn or make use of information from the system, *but does not affect system resources* (eg. eavesdropping, monitoring transmissions) 
    * are difficult to detect
    * prevent using encryption rather than worrying about detection
* Types of passive attacks:
    1. **Release of Message Contents:** attacker will monitors an unprotected communications  intercept it for sensitive information (eg.unencrypted email or telephone call) [[7](https://www.venafi.com/blog/what-active-attack-vs-passive-attack-using-encryption#:~:text=Release%20of%20message%20contents%3A%20In,intercept%20it%20for%20sensitive%20information.)]
    2. **Traffic Analysis:** hacker tries to access the same network and listen/capture and analyze your network traffic as it moves to and from the target systems [[8](https://www.netreo.com/blog/traffic-analysis-attack/)] [[9](https://www.techtarget.com/whatis/definition/passive-attack#:~:text=Passive%20attacks%20can%20take%20various,communication%20exchanged%20over%20the%20network.)]; use statistical methods to analyze and interpret the patterns of communication exchanged over the network [[9](https://www.techtarget.com/whatis/definition/passive-attack#:~:text=Passive%20attacks%20can%20take%20various,communication%20exchanged%20over%20the%20network.)]
        * eg. could observe and determine location/identity of hosts and observe frequency/length of message exchange
#### Active Attacks
#### Figure 1.3 Active Network Security Attacks Dissection 

