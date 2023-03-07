# Module 1: Understand Data Security

Domain D5.0, D5.1.1, D5.1.2, D5.1.3

#### Module Objective

-   L5.0 Explain concepts of security operations.
-   L5.1.1 Discuss data handling best practices.
-   L5.1.2 Identify key concepts of logging and monitoring.
-   L5.1.3 Summarize the different types of encryption and their common uses

**Hardening** (def: A reference to the process of applying secure configurations (to reduce the attack surface) and locking down various hardware, communications systems, and software, including operating system, web server, application server, application, etc. Hardening is normally performed based on industry guidelines and benchmarks, such as those provided by the Center for Internet Security (CIS).) is the process of applying secure configurations (to reduce the attack surface) and locking down various hardware, communications systems and software, including the **operating system**,**web server** "A computer that provides World Wide Web (WWW) services on the Internet. It includes the hardware, operating system, Web server software, and Web site content (Web pages). If the Web server is used internally and not by the public, it may be known as an “intranet server.”"), **application server**(A computer responsible for hosting applications to user workstations.) and applications, etc. In this module, we will introduce configuration management practices that will ensure systems are installed and maintained according to industry and organizational security standards.

video UnderstandDataSecurity.mkv

transcripts
Manny: It's hard to imagine the sheer volume of data that's flying around the world right now. Tasha: Right, and information security, as a process and discipline, provides a structure for protecting the value of data. As an organization creates, stores, shares, uses, modifies, archives, and finally destroys that data. Manny: Writing information down on paper, a whiteboard, or a flash drive, or putting it in a file on Cloud creates data that is a tangible asset. The organization has to protect both the ideas and the data. Tasha: Yes, and all the copies of it in papers, books, conversation logs, computer files, database records and the network packets which help move that information from one location or user to another. Manny: Wow, that's an important job. Tasha: It sure is.


# Data Handling

Data itself goes through its own life cycle as users create, use, share and modify it. Many different models of the life of a data item can be found, but they all have some basic operational steps in common. The data security life cycle model is useful because it can align easily with the different roles that people and organizations perform during the evolution of data from creation to destruction (or disposal). It also helps put the different data states of in use, at rest and in motion, into context. Let’s take a closer look. 

All ideas, data, information or knowledge can be thought of as going through six major sets of activities throughout its lifetime. Conceptually, these involve:
Select a hot spot to learn more.![[2023-03-07 12_19_01-Data Handling.png]]

##### Create
Creating the knowledge, which is usually tacit knowledge at this point.

##### Store
Storing or recording it in some fashion (which makes it explicit).

##### Use
Using the knowledge, which may cause the information to be modified, supplemented or partially deleted.

##### Share
Sharing the data with other users, whether as a copy or by moving the data from one location to another.

##### Archive
Archiving the data when it is temporarily not needed.

##### Destroy
Destroying the data when it is no longer needed.


# Data Handling Deeper Dive video
 video  DataHandlingDeeper.mkv

[Download Transcript](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/transcripts/Data%20Handling%20Deeper%20Dive.pdf?_&d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541)
Narrator: Data handling is extremely important. As soon as we receive the assets, the data we need to protect, we need to make sure we know the best practices for handling this data. First, we need to recognize which assets we need to protect. This is based on the value of the data according to the owner of that data. Based on that, we see what kind of risk we are facing with respect to the likelihood that this information could be compromised, destroyed or changed by any means, and what vulnerabilities exist that we need to account for. This is the life cycle of data handling, from create, to store, to use, to share, to archive and finally to destroy. And at any point there are different risks to the data and different practices for handling it. Some of these procedures are mandated by government standards. For example, in the US, the Occupational Safety and Health Administration (OSHA) is the federal government agency that protects the well-being of workers. Under the rules of the Healthcare Insurance Portability and Accountability Act (HIPAA), medical records need to be kept for 10 years, but under OSHA, if we have a medical record of an on-the-job injury, that record needs to be maintained for over 30 years, even after the last day of work in that particular organization. That’s a regulatory requirement, and if you don’t know that or don’t abide by it, you can find yourself in trouble as the result of an audit. So you can see that we have to be very cautious when deciding how to handle data, as there may be multiple regulations that apply to a single piece of data. Also in the US there are also specific guidelines related to the Payment Card Industry Data Security Standards (PCI DSS) requirements regarding credit card information and how to maintain that information securely. In the European Union, the GDPR also has specific requirements regarding the handling of financial data. In order to protect the data properly, you need to know all the relevant requirements for the type of data being protected in the various geographic areas. Many countries and other jurisdictions have regulations that require certain data protections throughout every stage of the data’s life cycle. These govern how the data is acquired, processed, stored, and ultimately destroyed. And when looking at the life cycle of the data, we need to keep a watchful eye and protect the information at every stage, even if it’s ready to be legally destroyed at the end of the life cycle. In some cases, multiple jurisdictions may impose rules affecting the data we are charged with protecting. In these instances, we need to be aware of any and all regulations that affect us. Some data handling practices include classification and labeling, where you determine the sensitivity of the data, what is available to everyone and what needs to be restricted, and label the information accordingly so that your access controls will allow the correct level of access. Retention is how long we store the information and where, based on the requirements of our organization and perhaps regulatory agencies as well. And then there needs to be defensible destruction, meaning that we have the regulatory mandate backing up our decision to destroy the data. Destruction can be physical, of hard drives or computer chips, or destruction of digital records, which can be done under a number of methodologies. We need to make sure we understand the secure destruction of the data, because often we think we can just empty the virtual trash can to delete the data. But when we do that, old emails and other data may never be erased. To completely erase the data on physical media, you need to use some technical equipment for degaussing, such as powerful magnets to erase the data stored on tape and disk media such as computer and laptop hard drives, diskettes, reels, cassettes and cartridge tapes. However, an individual with sophisticated equipment could potentially still retrieve that information, at least partially. So we must make sure we understand what recovery tools are available, because if you are subject to regulatory compliance, you have to follow through with specific protocols and processes to destroy that information as required so that it can no longer be accessed in any way.


# Data Handling Practices

Data itself has value and must be handled appropriately.  In this section, we will explore the basics of classifying and labeling data to ensure it is treated and controlled in a manner consistent with the sensitivity of the data. In addition, we will complete the data life cycle by documenting retention requirements and ensuring data that is no longer in use is destroyed. 

## ![image of file folder with document and magnifying glass](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/assets/img/EDU-ELCC-70435-Classification-techart-v02.svg?_&d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541 "image of file folder with document and magnifying glass") Classification

Businesses recognize that information has value and others might steal their advantage if the information is not kept confidential, so they classify it. These classifications dictate rules and restrictions about how that information can be used, stored or shared with others. All of this is done to keep the temporary value and importance of that information from leaking away. Classification of data, which asks the question “Is it secret?” determines the labeling, handling and use of all data. 

Before any labels can be attached to sets of data that indicate its sensitivity or handling requirements, the potential impact or loss to the organization needs to be assessed. This is our first definition: Classification (DEF : _Classification identifies the degree of harm to the organization, its stakeholders or others that might result if an information asset is divulged to an unauthorized person, process or organization. In short, classification is focused first and foremost on maintaining the confidentiality of the data, based on the data sensitivity._) is the process of recognizing the organizational impacts if the information suffers any security compromises related to its characteristics of confidentiality, integrity and availability. Information is then labeled and handled accordingly. 

Classifications are derived from laws, regulations, contract-specified standards or other business expectations. One classification might indicate “minor, may disrupt some processes” while a more extreme one might be “grave, could lead to loss of life or threaten ongoing existence of the organization.” These descriptions should reflect the ways in which the organization has chosen (or been mandated) to characterize and manage risks.  

The immediate benefit of classification is that it can lead to more efficient design and implementation of security processes, if we can treat the protection needs for all similarly classified information with the same controls strategy.

## ![image of file folder with label](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/assets/img/EDU-ELCC-70420-Labeling-techart-v02.svg?_&d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541 "image of file folder with label") Labeling

Security labels are part of implementing controls to protect classified information. It is reasonable to want a simple way of assigning a level of sensitivity to a data asset, such that the higher the level, the greater the presumed harm to the organization, and thus the greater security protection the data asset requires. This spectrum of needs is useful, but it should not be taken to mean that clear and precise boundaries exist between the use of “low sensitivity” and “moderate sensitivity” labeling, for example. 

### Data Sensitivity Levels and Labels 

Unless otherwise mandated, organizations are free to create classification systems that best meet their own needs. In professional practice, it is typically best if the organization has enough classifications to distinguish between sets of assets with differing sensitivity/value, but not so many classifications that the distinction between them is confusing to individuals. Typically, two or three classifications are manageable, and more than four tend to be difficult. 

-   Highly restricted: Compromise of data with this sensitivity label could possibly put the organization’s future existence at risk. Compromise could lead to substantial loss of life, injury or property damage, and the litigation and claims that would follow.
-   Moderately restricted: Compromise of data with this sensitivity label could lead to loss of temporary competitive advantage, loss of revenue or disruption of planned investments or activities.
-   Low sensitivity (sometimes called “internal use only”): Compromise of data with this sensitivity label could cause minor disruptions, delays or impacts.
-   Unrestricted public data: As this data is already published, no harm can come from further dissemination or disclosure.
## Retention

Information and data should be kept only for as long as it is beneficial, no more and no less. For various types of data, certain industry standards, laws and regulations define retention periods. When such external requirements are not set, it is an organization’s responsibility to define and implement its own data retention policy. Data retention policies are applicable both for hard copies and for electronic data, and no data should be kept beyond its required or useful life. Security professionals should ensure that data destruction is being performed when an asset has reached its retention limit. For the security professional to succeed in this assignment, an accurate inventory must be maintained, including the asset location, retention period requirement, and destruction requirements. Organizations should conduct a periodic review of retained [records](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/module_01/ch05_m01-Data_Handling_Practices.html?d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541&d2l_body_type=3#) in order to reduce the volume of information stored and to ensure that only necessary information is preserved. 

**Records retention**( _Def:A practice based on the records life cycle, according to which records are retained as long as necessary, and then are destroyed after the appropriate time interval has elapsed_.) policies indicate how long an organization is required to maintain information and assets. Policies should guarantee that: 

-   Personnel understand the various retention requirements for data of different types throughout the organization. 
-   The organization appropriately documents the retention requirements for each type of information.
-   The systems, processes and individuals of the organization retain information in accordance with the required schedule but no longer. 

A common mistake in records retention is applying the longest retention period to all types of information in an organization. This not only wastes storage but also increases risk of data exposure and adds unnecessary “noise” when searching or processing information in search of relevant records. It may also be in violation of externally mandated requirements such as legislation, regulations or contracts (which may result in fines or other judgments). Records and information no longer mandated to be retained should be destroyed in accordance with the policies of the enterprise and any appropriate legal requirements that may need to be considered.

## Destruction

Data that might be left on media after deleting is known as **remanence** (_def: Residual information remaining on storage media after clearing. NIST SP 800-88 Rev. 1_) and may be a significant security concern. Steps must be taken to reduce the risk that data remanence could compromise sensitive information to an acceptable level. This can be done by one of several means:  

-   Clearing the device or system, which usually involves writing multiple patterns of random values throughout all storage media (such as main memory, registers and fixed disks). This is sometimes called “overwriting” or “zeroizing” the system, although writing zeros has the risk that a missed block or storage extent may still contain recoverable, sensitive information after the process is completed.
-   Purging the device or system, which eliminates (or greatly reduces) the chance that residual physical effects from the writing of the original data values may still be recovered, even after the system is cleared. Some magnetic disk storage technologies, for example, can still have residual “ghosts” of data on their surfaces even after being overwritten multiple times. Magnetic media, for example, can often be altered sufficiently to meet security requirements; in more stringent cases, **degaussing**(_def: A technique of erasing data on disk or tape (including video tapes) that, when performed properly, ensures that there is insufficient magnetic remanence to reconstruct data._) may not be sufficient. 
-   Physical destruction of the device or system is the ultimate remedy to data remanence. Magnetic or optical disks and some flash drive technologies may require being mechanically shredded, chopped or broken up, etched in acid or burned; their remains may be buried in protected landfills, in some cases.

In many routine operational environments, security considerations may accept that clearing a system is sufficient. But when systems elements are to be removed and replaced, either as part of maintenance upgrades or for disposal, purging or destruction may be required to protect sensitive information from being compromised by an attacker.

# Logging and Monitoring Security Events

Logging is the primary form of instrumentation that attempts to capture signals generated by events. Events are any actions that take place within the systems environment and cause measurable or observable change in one or more elements or resources within the system. Logging imposes a computational cost but is invaluable when determining accountability. Proper design of logging environments and regular log reviews remain best practices regardless of the type of computer system. 

Major controls frameworks emphasize the importance of organizational logging practices. Information that may be relevant to being recorded and reviewed include (but is not limited to): 

-   user IDs
-   system activities
-   dates/times of key events (e.g., logon and logoff)
-   device and location identity
-   successful and rejected system and resource access attempts
-   system configuration changes and system protection activation and deactivation events 

 Logging and monitoring the health of the information environment is essential to identifying inefficient or improperly performing systems, detecting compromises and providing a record of how systems are used. Robust logging practices provide tools to effectively correlate information from diverse systems to fully understand the relationship between one activity and another. 

Log reviews are an essential function not only for security assessment and testing but also for identifying security incidents, policy violations, fraudulent activities and operational problems near the time of occurrence. Log reviews support audits – forensic analysis related to internal and external investigations – and provide support for organizational security baselines. Review of historic audit logs can determine if a vulnerability identified in a system has been previously exploited. 

It is helpful for an organization to create components of a log management infrastructure and determine how these components interact. This aids in preserving the integrity of log data from accidental or intentional modification or deletion and in maintaining the confidentiality of log data. 

Controls are implemented to protect against unauthorized changes to log information. Operational problems with the logging facility are often related to alterations to the messages that are recorded, log files being edited or deleted, and storage capacity of log file media being exceeded. Organizations must maintain adherence to retention policy for logs as prescribed by law, regulations and corporate governance. Since attackers want to hide the evidence of their attack, the organization’s policies and procedures should also address the preservation of original logs. Additionally, the logs contain valuable and sensitive information about the organization.  Appropriate measures must be taken to protect the log data from malicious use. 

## Events

![Screenshot of a log](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/assets/img/EDU-ELCC-70440-log-v01.png?_&d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541 "Screenshot of a log")

## Event Detail

![Screenshot of an event on the log](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/assets/img/EDU-ELCC-70445-event_on_log-v01.png?_&d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541 "Screenshot of an event on the log")

## Raw Log (Also shown at the bottom of event detail)

![Screenshot of an incident on the log](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/assets/img/EDU-ELCC-70450-incident_on_log-v01.png?_&d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541 "Screenshot of an incident on the log")

# Data Security Event Example

Here is a data security event example. It’s a raw log, and it is one way to see if someone tried to break into a secure file and hijack the server. Of course, there are other systems now that are a little more user-friendly. But security engineers get very familiar with some of these codes and can figure out exactly who was trying to log it, was it a secure port or a questionable port that they were trying to use to penetrate our site. 

Information security is not something that you just plug in as needed. You can have some patching on a system that already exists, such as updates, but if you don’t have a secure system, you can’t just plug in something to protect it. From the very beginning, we need to plan for that security, even before the data is introduced into the network. 

![Image of a raw data log](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/assets/img/EDU-CCSP-71155-image-raw_log-v01.png?_&d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541 "Image of a raw data log")

# Event Logging Best Practices

Different tools are used depending on whether the risk from the attack is from traffic coming into or leaving the infrastructure. **Ingress monitorin**(_def:Monitoring of incoming network traffic._) refers to surveillance and assessment of all inbound communications traffic and access attempts. Devices and tools that offer logging and alerting opportunities for ingress monitoring include: 

-   Firewalls
-   Gateways
-   Remote authentication servers
-   IDS/IPS tools
-   SIEM solutions
-   Anti-malware solutions

**Egress monitoring**(_def:Monitoring of outgoing network traffic._) is used to regulate data leaving the organization’s IT environment. The term currently used in conjunction with this effort is **data loss prevention (DLP)**(_System capabilities designed to detect and prevent the unauthorized use and transmission of information._) or data leak protection. The DLP solution should be deployed so that it can inspect all forms of data leaving the organization, including: 

-   Email (content and attachments)
-   Copy to portable media
-   File Transfer Protocol (FTP)
-   Posting to web pages/websites
-   Applications/application programming interfaces (APIs)

# Logging

Which of the following does not normally influence an organization’s retention policy for logs? (D5, L5.1.3) 

 A. Laws

 B. Audits

 C. Corporate governance

 D. Regulations

Check Answer

Correct answer: B. Audits

Audits are a way to measure compliance with policy, but do not normally influence the retention policy itself. Organizations must maintain adherence to retention policy for logs as prescribed by law, regulations and corporate governance.


# Encryption Overview

Almost every action we take in our modern digital world involves **cryptography**(_The study or applications of methods to secure or protect the meaning and content of messages, files, or other information, usually by disguise, obscuration, or other transformations of that content and meaning._). 
>[!Encryption]- 
>The process and act of converting the message from its plaintext to ciphertext. Sometimes it is also referred to as enciphering. The two terms are sometimes used interchangeably in literature and have similar meanings.

protects our personal and business transactions; digitally signed software updates verify their creator’s or supplier’s claim to authenticity. Digitally signed contracts, binding on all parties, are routinely exchanged via email without fear of being repudiated later by the sender. 

Cryptography is used to protect information by keeping its meaning or content secret and making it unintelligible to someone who does not have a way to decrypt (unlock) that protected information. The objective of every encryption system is to transform an original set of data, called the plaintext, into an otherwise unintelligible encrypted form, called the **ciphertext**(_The altered form of a plaintext message so it is unreadable for anyone except the intended recipients. In other words, it has been turned into a secret._). 

Properly used, singly or in combination, cryptographic solutions provide a range of services that can help achieve required systems security postures in many ways: 

-   Confidentiality: Cryptography provides confidentiality by hiding or obscuring a message so that it cannot be understood by anyone except the intended recipient. Confidentiality keeps information secret from those who are not authorized to have it. 
-   Integrity: **hash functions**(_def: An algorithm that computes a numerical value (called the hash value) on a data file or electronic message that is used to represent that file or message and depends on the entire contents of the file or message. A hash function can be considered to be a fingerprint of the file or message. NIST SP 800-152_) and **digital signatures** (_The result of a cryptographic transformation of data which, when properly implemented, provides the services of origin authentication, data integrity, and signer non-repudiation. NIST SP 800-12 Rev. 1_) can provide integrity services that allow a recipient to verify that a message has not been altered by malice or error. These include simple message integrity controls. Any changes, deliberate or accidental, will result in the two results (by sender and by recipient) being different.
- ![[2023-03-07 12_59_05-Encryption Overview.png]]
- An **encryption system**(_The total set of algorithms, processes, hardware, software, and procedures that taken together provide an encryption and decryption capability._) is the set of hardware, software, algorithms, control parameters and operational methods that provide a set of encryption services.

**Plaintext** is the data or message in its normal, unencrypted form and format. Its meaning or value to an end user (a person or a process) is immediately available for use.

Plaintext can be:

-   image, audio or video files in their raw or compressed forms
-   human-readable text and numeric data, with or without markup language elements for formatting and metadata
-   database files or records and fields within a database
-   or anything else that can be represented in digital form for computer processing, transmission and storage

It is important to remember that plaintext can be anything—much of which is not readable to humans in the first place.
## Symmetric Encryption

The central characteristic of a symmetric algorithm is that it uses the same key in both the encryption and the decryption processes. It could be said that the 
>[!**decryption**]-
>(def: _The reverse process from encryption. It is the process of converting a ciphertext message back into plaintext through the use of the cryptographic algorithm and the appropriate key for decryption (which is the same for symmetric encryption, but different for asymmetric encryption). This term is also used interchangeably with the “deciphering.”_ )

process is just a mirror image of the encryption process. 
This image displays how symmetric algorithms work.
![[2023-03-07 13_07_12-Encryption Overview.png]]

The same key is used for both the encryption and decryption processes. This means that the two parties communicating need to share knowledge of the same key. This type of algorithm protects data, as a person who does not have the correct key would not be able to read the encrypted message. Because the key is shared, however, this can lead to several other challenges:

-   If two parties suspect a specific communication path between them is compromised, they obviously can't share key material along that path. Someone who has compromised communications between the parties would also intercept the key.

-   Distribution of the key is difficult, because the key cannot be sent in the same channel as the encrypted message, or the man-in-the-middle (MITM) would have access to the key. Sending the key through a different channel (band) than the encrypted message is called out-of-band key distribution. Examples of out-of-band key distribution would include sending the key via courier, fax or phone.
-   Any party with knowledge of the key can access (and therefore change) the message.
-   Each individual or group of people wishing to communicate would need to use a different key for each individual or group they want to connect with. This raises the challenge of scalability — the number of keys needed grows quickly as the number of different users or groups increases. Under this type of symmetric arrangement, an organization of 1,000 employees would need to manage 499,500 keys if every employee wanted to communicate confidentially with every other employee.

Primary uses of symmetric algorithms:
-   Encrypting bulk data (backups, hard drives, portable media)
-   Encrypting messages traversing communications channels (IPsec, TLS)
-   Streaming large-scale, time-sensitive data (audio/video materials, gaming, etc.)

Other names for symmetric algorithms, which you may encounter, include:

-   Same key
-   Single key
-   Shared key
-   Secret key
-   Session key

An example of [symmetric encryption](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/module_01/ch05_m01-Encryption_Overview.html?d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541&d2l_body_type=3#) is a substitution cipher, which involves the simple process of substituting letters for other letters, or more appropriately, substituting bits for other bits, based upon a cryptovariable. These ciphers involve replacing each letter of the plaintext with another that may be further down the alphabet.

##### Asymmetric Encryption

**Asymmetric encryption** (_def:An algorithm that uses one key to encrypt and a different key to decrypt the input plaintext._) uses one key to encrypt and a different key to decrypt the input plaintext. This is in stark contrast to symmetric encryption, which uses the same key to encrypt and decrypt. For most security professionals, the math of asymmetric encryption can be left to the **cryptanalysts** (_def: One who performs cryptanalysis which is the study of mathematical techniques for attempting to defeat cryptographic techniques and/or information systems security. This includes the process of looking for errors or weaknesses in the implementation of an algorithm or of the algorithm itself._) and cryptographers to know.

A user wishing to communicate using an asymmetric algorithm would first generate a key pair. To ensure the strength of the key generation process, this is usually done by the cryptographic application or the public key infrastructure (PKI) implementation without user involvement. One half of the key pair is kept secret; only the key holder knows that key. This is why it is called the private key. The other half of the key pair can be given freely to anyone who wants a copy. In many companies, it may be available through the corporate website or access to a key server. Therefore, this second half of the key pair is referred to as the public key.

Note that anyone can encrypt something using the recipient’s public key, but only the recipient —with their private key—can decrypt it.

Asymmetric key cryptography solves the problem of key distribution by allowing a message to be sent across an untrusted medium in a secure manner without the overhead of prior key exchange or key material distribution. It also allows for several other features not readily available in symmetric cryptography, such as the non-repudiation of origin and delivery, access control and data integrity.

Asymmetric key cryptography also solves the problem of scalability. It does scale well as numbers increase, as each party only requires a key pair, the private and public keys. An organization with 100,000 employees would only need a total of 200,000 keys (one private and one public for each employee). This is less than half of the number of keys that would be required for symmetric encryption.

The problem, however, has been that asymmetric cryptography is extremely slow compared with its symmetric counterpart. Asymmetric cryptography is impractical for everyday use in encrypting large amounts of data or for frequent transactions where speed is required. This is because asymmetric key cryptography is handling much larger keys and is mathematically intensive, thereby reducing the speed significantly.

Let’s look at an example that illustrates the use of asymmetric cryptography to achieve different security attributes.
![[2023-03-07 13_11_11-Encryption Overview.png]]

The two keys (private and public) are a key pair; they must be used together. This means that any message that is encrypted with a public key can only be decrypted with the corresponding other half of the key pair, the private key. Similarly, signing a message with a sender’s private key can only be verified by the recipient decrypting its signature with the sender’s public key. Therefore, as long as the key holder keeps the private key secure, there exists a method of transmitting a message confidentially. The sender would encrypt the message with the public key of the receiver. Only the receiver with the private key would be able to open or read the message, providing confidentiality.

This image shows how asymmetric encryption can be used to send a confidential message across an untrusted channel.

## Encryption Deeper Dive video

EncryptionDeeperDive.mkv
transcript
Narrator: Examples of encryption persist throughout human history, from early cryptic depictions by cave dwellers of Magura Cave in Bulgaria to the Pyramids at Giza. Even then, each group had its own primitive cryptographic approach, so that members of the tribe or group could communicate with one another while keeping secrets from the rival tribes regarding hunting grounds or sources of water and food. It is part of human nature to encrypt information. You start with clear text, which is the information that you and I could easily read, and then you use an algorithm, which is often a form of software that can be embedded in the system. But that needs to be activated with an encryption key. A very simple example is if you are trying to encrypt a PDF document; for example, perhaps your accountant is sending you some documents to sign before submitting your taxes. Encryption would create a ciphertext, which no one can use, and you and your accountant would have set up a preset encryption key so that you could retrieve the information at either end of the communication. You need to have good key management, which means you safeguard the information, because imagine if you have thousands of keys in a commercial environment. There is often a third party or external server where the keys will be separately stored and managed, so you don’t have all your eggs in one basket, so to speak. It will be protected through a hashing system, which we will explore in a moment, and no one else can have access to those keys. Asymmetric encryption is more secure because the sender and receiver each uses a unique code, often a certificate, so you can confirm that the information has been sent from the sender to the recipient in a secure manner

## Hashing

**Hashing**(_def: The process of using a mathematical algorithm against data to produce a numeric value that is representative of that data. Source CNSSI 4009-2015_) takes an input set of data (of almost arbitrary size) and returns a fixed-length result called the hash value. A hash function is the algorithm used to perform this transformation. When used with cryptographically strong hash algorithms, this is the most common method of ensuring message integrity today.

Hashes have many uses in computing and security, one of which is to create a **message digest** (_def: A digital signature that uniquely identifies data and has the property such that changing a single bit in the data will cause a completely different message digest to be generated. NISTIR-8011 Vol.3_) by applying such a hash function to the plaintext body of a message. 

To be useful and secure, a cryptographic hash function must demonstrate five main properties: 

-   Useful: It is easy to compute the hash value for any given message.
-   Nonreversible: It is computationally infeasible to reverse the hash process or otherwise derive the original plaintext of a message from its hash value (unlike an encryption process, for which there must be a corresponding decryption process).
-   Content integrity assurance: It is computationally infeasible to modify a message such that re-applying the hash function will produce the original hash value. 
-   Unique: It is computationally infeasible to find two or more different, sensible messages that hash to the same value.
-   Deterministic: The same input will always generate the same hash, when using the same hashing algorithm.
Cryptographic hash functions have many applications in information security, including digital signatures, message authentication codes and other forms of authentication. They can also be used for fingerprinting, to detect duplicate data or uniquely identify files, and as **checksums** (_A digit representing the sum of the correct digits in a piece of stored or transmitted digital data, against which later comparisons can be made to detect errors in the data._) to detect accidental data corruption. The operation of a hashing algorithm is demonstrated in this image.
![[2023-03-07 13_23_01-Encryption Overview.png]]
This is an example of a simple hashing function. The originator wants to send a message to the receiver and ensure that the message is not altered by noise or lost packets as it is transmitted. The originator runs the message through a hashing algorithm that generates a hash, or a digest of the message. The digest is appended to the message and sent together with the message to the recipient. Once the message is delivered, the receiver will generate their own digest of the received message (using the same hashing algorithm). The digest of the received message is compared with the digest sent by the originator. If the digests are the same, the received message is the same as the sent message.

The problem with a simple hash function like this is that it does not protect against a malicious attacker that would be able to change both the message and the hash/digest by intercepting it in transit. The general idea of a cryptographic hash function can be summarized with the following formula:

 

variable data input + hashing algorithm

= fixed bit size data output (the digest)


even the slightest change in the input message results in a completely different hash value.

Hash functions are very sensitive to any changes in the message. Because the size of the hash digest does not vary according to the size of the message, a person cannot tell the size of the message based on the digest.

# How Passwords Work video

 HowPasswordsWork.mkv


[Download Transcript](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_05/transcripts/How%20Passwords%20Work.pdf?_&d2lSessionVal=cvTrTCqN5CaEQU1Bv8rdyg8eF&ou=9541)
Narrator: Often your password will be stored as a fixed hash value or digest, so that the system can tell if your password matches without the password itself ever being visible. A more secure password with alphanumeric and special characters will generate a different type of hash digest. However, this system of password management is already becoming obsolete. Often, for security purposes, you will be asked to generate a new password with a minimum number of characters, and the software behind it will recognize the hash function and tell you if the password is sufficiently secure to be used, or it will prompt you to create a better password. Attackers can use password hashes to “guess” your password offline. If an attacker can copy the password file, which is usually hashed, from a compromised workstation or server, and they know the algorithm that is used to hash the password, they can use a computer to try random sequences of letters and number combinations to try to match the known password hash.


