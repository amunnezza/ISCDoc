
# Module 5: Chapter 5 Summary

Domain 5.1.1, 5.1.2, 5.1.3, 5.2.1, 5.3.1, 5.3.2, 5.3.3, 5.3.4, 5.3.6, 5.4.1, 5.4.2 

## Module Objective

L5.5.1 Practice the terminology and review concepts of access controls  

This chapter focused on the day-to-day, moment-by-moment, use of security controls and risk mitigation strategies in an organization. We discovered ways to secure data and the systems they reside on. Data (information) security as a process and discipline provides a structure for protecting the value of data as the organization creates, stores, shares, uses, modifies, archives and finally destroys that data (known as data handling). During data handling, an organization classifies (assigns data sensitivity levels), categorizes (determines type of data), labels (applies a name to the data), retains (determines how long to keep the data) and destroys (erases or destroys) the data.  

A best practice for securing data is encrypting the data. We explored the process of encrypting data in plaintext with a key and algorithm to create ciphertext then using either the same key (symmetric) or a different key (asymmetric) and same algorithm to decrypt the ciphertext to convert it back to plaintext. Then hashing was methodically described; hashing takes an input set of data (of almost arbitrary size) and returns a fixed-length result called the hash value.  

System hardening is the process of applying secure configurations (to reduce the attack surface) and locking down various hardware, communications systems and software, including operating system, web server, application server, application, etc. We also discussed configuration management, a process and discipline used to ensure that the only changes made to a system are those that have been authorized and validated. Configuration management consists of identification, baseline, change control, and verification and audit. During configuration management, one must conduct inventory, baselines, updates, and patches.  

The following best practice security policies were examined: data handling (appropriate use of data), password (appropriate use of passwords), acceptable use (appropriate use of the assets, devices, and data), bring your own device (appropriate use of personal devices), privacy (appropriate protection of one’s privacy), and change management (appropriate transition from current state to a future state). Change management practices address a common set of core activities: documentation, approval, and rollback. It starts with a request for change (RFC) and moves through various development and test stages until the change is released to the end users. 

We ended the chapter by discussing the importance of security awareness training and how it reduces the internal threat to an organization. By breaking down the levels of security awareness training into education, training, and awareness, we identified that the training can be tailored to the security topic(s), organization, position and/or individual. The module highlighted some of the main threats, including phishing and social engineering and why it's important to include them in your security awareness training programs. We also emphasized the importance of password protection.
****

# Chapter 5: Terms and Definitions
_Click on each tab to learn more._ 

[A - C]()
- **Application Server** - A computer responsible for hosting applications to user workstations. NIST SP 800-82 Rev.2
-   **Asymmetric Encryption** - An algorithm that uses one key to encrypt and a different key to decrypt the input plaintext.
-   **Checksum** - A digit representing the sum of the correct digits in a piece of stored or transmitted digital data, against which later comparisons can be made to detect errors in the data.
-   **Ciphertext** - The altered form of a plaintext message so it is unreadable for anyone except the intended recipients. In other words, it has been turned into a secret.
-   **Classification** - Classification identifies the degree of harm to the organization, its stakeholders or others that might result if an information asset is divulged to an unauthorized person, process or organization. In short, classification is focused first and foremost on maintaining the confidentiality of the data, based on the data sensitivity.
-   **Configuration management** - A process and discipline used to ensure that the only changes made to a system are those that have been authorized and validated.
-   **Cryptanalyst** - One who performs cryptanalysis which is the study of mathematical techniques for attempting to defeat cryptographic techniques and/or information systems security. This includes the process of looking for errors or weaknesses in the implementation of an algorithm or of the algorithm itself.
-   **Cryptography** - The study or applications of methods to secure or protect the meaning and content of messages, files, or other information, usually by disguise, obscuration, or other transformations of that content and meaning.
[D - E]()
-   **Data Loss Prevention (DLP)** - System capabilities designed to detect and prevent the unauthorized use and transmission of information. 
-   **Decryption** - The reverse process from encryption. It is the process of converting a ciphertext message back into plaintext through the use of the cryptographic algorithm and the appropriate key for decryption (which is the same for symmetric encryption, but different for asymmetric encryption). This term is also used interchangeably with the “deciphering.”
-   **Degaussing** - A technique of erasing data on disk or tape (including video tapes) that, when performed properly, ensures that there is insufficient magnetic remanence to reconstruct data.
-   **Digital Signature** - The result of a cryptographic transformation of data which, when properly implemented, provides the services of origin authentication, data integrity, and signer non-repudiation. NIST SP 800-12 Rev. 1
-   **Egress Monitoring** - Monitoring of outgoing network traffic.
-   **Encryption** - The process and act of converting the message from its plaintext to ciphertext. Sometimes it is also referred to as enciphering. The two terms are sometimes used interchangeably in literature and have similar meanings.
-   **Encryption System** - The total set of algorithms, processes, hardware, software, and procedures that taken together provide an encryption and decryption capability.

[F - O]()
-   **Hardening** - A reference to the process of applying secure configurations (to reduce the attack surface) and locking down various hardware, communications systems, and software, including operating system, web server, application server, application, etc. Hardening is normally performed based on industry guidelines and benchmarks, such as those provided by the Center for Internet Security (CIS).
-   **Hash Function** - An algorithm that computes a numerical value (called the hash value) on a data file or electronic message that is used to represent that file or message and depends on the entire contents of the file or message. A hash function can be considered to be a fingerprint of the file or message. NIST SP 800-152
-   **Hashing** - The process of using a mathematical algorithm against data to produce a numeric value that is representative of that data. Source CNSSI 4009-2015
-   **Ingress Monitoring** - Monitoring of incoming network traffic.
-   **Message Digest** - A digital signature that uniquely identifies data and has the property such that changing a single bit in the data will cause a completely different message digest to be generated. NISTIR-8011 Vol.3
-   **Operating System** - The software “master control application” that runs the computer. It is the first program loaded when the computer is turned on, and its main component, the kernel, resides in memory at all times. The operating system sets the standards for all application programs (such as the Web server) that run in the computer. The applications communicate with the operating system for most user interface and file management operations. NIST SP 800-44 Version 2

[P - R]()

-   **Patch** - A software component that, when installed, directly modifies files or device settings related to a different software component without changing the version number or release details for the related software component. Source: ISO/IEC 19770-2
-   **Patch Management** - The systematic notification, identification, deployment, installation and verification of operating system and application software code revisions. These revisions are known as patches, hot fixes, and service packs. Source: CNSSI 4009
-   **Plaintext** - A message or data in its natural format and in readable form; extremely vulnerable from a confidentiality perspective.
-   **Records** - The recordings (automated and/or manual) of evidence of activities performed or results achieved (e.g., forms, reports, test results), which serve as a basis for verifying that the organization and the information system are performing as intended. Also used to refer to units of related data fields (i.e., groups of data fields that can be accessed by a program and that contain the complete set of information on particular items). NIST SP 800-53 Rev. 4
-   **Records Retention** - A practice based on the records life cycle, according to which records are retained as long as necessary, and then are destroyed after the appropriate time interval has elapsed.
-   **Remanence** - Residual information remaining on storage media after clearing. NIST SP 800-88 Rev. 1
-   **Request for change (RFC)** - The first stage of change management, wherein a change in procedure or product is sought by a stakeholder.

[S - Z]()
-   **Security Governance** - The entirety of the policies, roles, and processes the organization uses to make security decisions in an organization.
-   **Social engineering** - Tactics to infiltrate systems via email, phone, text, or social media, often impersonating a person or agency in authority or offering a gift. A low-tech method would be simply following someone into a secure building.
-   **Symmetric encryption** - An algorithm that uses the same key in both the encryption and the decryption processes.
-   **Web Server** - A computer that provides World Wide Web (WWW) services on the Internet. It includes the hardware, operating system, Web server software, and Web site content (Web pages). If the Web server is used internally and not by the public, it may be known as an “intranet server.” NIST SP 800-44 Version 2
-   **Whaling Attack** - Phishing attacks that attempt to trick highly placed officials or private individuals with sizable assets into authorizing large fund wire transfers to previously unknown entities.
****

# Chapter 5: Glossary Flash Cards
fare

  ****
  # Summary

## Description

This quiz will help you to confirm your understanding and retention of concepts for this chapter. Please complete it by answering all questions, reviewing correct answers and feedback, and revisiting any chapter material you feel you need extra time with.

**Instructions**

1.  This Assessment contains 10 objective item questions.
2.  Recommended time limit is 20 minutes, 2 minutes per question.
3.  Choose the best answer(s) for each question.
4.  You have unlimited attempts and may complete this assessment as many times as you would like.
5.  Passing grade for this quiz is 70%.
6.  Score of highest attempt will be calculated.

**Your score and quiz report**

1.  Each question carries 1 point.
2.  For each question, a 1/1 point indicates correct answer and 0/1 point indicates incorrect answer which you see upon quiz submission.
3.  Upon completion, you will be able to see your total number of attempts along with the score for each attempt.
4.  Your overall grade reflects the score of your highest attempt.
5.  Click on each attempt to view the completed quiz.

## Quiz Details

Current Time

6:59 AM

Update

Current User

luciano ciotola (username: luciociotola@gmail.com)

Time Allowed

Unlimited (estimated time required: 0:20:00)

Attempts

Allowed - Unlimited, Completed - 0

Activity Completion Condition

Score at least **70%** to pass the quiz and complete the activity.

## Instructions

Before you submit the quiz, you will have the opportunity to return to questions that you may have missed or have not yet answered.

You can submit your quiz responses at any time.

Click "Start Quiz" to begin Attempt 1.

**The timer will not begin until after the set up process is finished.**

## luciano ciotola (username: luciociotola@gmail.com)

## Attempt 1

Written: Mar 18, 2023 6:59 AM - Mar 18, 2023 7:07 AM

## Submission View

Your quiz has been submitted successfully.

**Question 1**

1 / 1 point

Which of the following can be used to map data flows through an organization and the relevant security controls used at each point along the way? (D5.1, L5.1.1)

Question options:

A) 

Encryption

B) 

Hashing

C) 

Hard copy

D) 

Data life cycle

Hide question 1 feedback

Correct. The data life cycle is a notional tool that can be used to map data flows. 

**Question 2**

1 / 1 point

Why is an asset inventory so important? (D5.2, L5.2.1)

Question options:

A) 

It tells you what to encrypt

B) 

You can't protect what you don't know you have

C) 

The law requires it 

D) 

 It contains a price list

Hide question 2 feedback

Correct. The inventory records which assets the organization has, which gives the organization the opportunity to protect those assets.

**Question 3**

1 / 1 point

Who is responsible for publishing and signing the organization's policies? (D5.3, L5.3.1)

Question options:

A) 

The security office

B) 

Human Resources

C) 

Senior management

D) 

The legal department

Hide question 3 feedback

Correct. Policies are direct organizational mandates from senior management. 

**Question 4**

1 / 1 point

Which of the following is always true about logging? (D5.1, L5.1.3) 

Question options:

A) 

Logs should be very detailed 

B) 

Logs should be in English

C) 

Logs should be concise

D) 

Logs should be stored separately from the systems they're logging

Hide question 4 feedback

Correct. It is important to store log data somewhere other than on the machine where the data is gathered.

**Question 5**

1 / 1 point

A mode of encryption for ensuring confidentiality efficiently, with a minimum amount of processing overhead (D5.1, L5.1.3) 

Question options:

A) 

Asymmetric

B) 

Symmetric

C) 

Hashing

D) 

Covert

Hide question 5 feedback

Correct. Symmetric encryption provides confidentiality with the least amount of processing overhead. 

**Question 6**

1 / 1 point

A ready visual cue to let anyone in contact with the data know what the classification is. (D5.1, L5.1.1)

Question options:

A) 

Encryption

B) 

Label

C) 

Graphics

D) 

Photos

Hide question 6 feedback

Correct. The label reflects the classification of a given piece of data.

**Question 7**

1 / 1 point

A set of security controls or system settings used to ensure uniformity of configuration throughout the IT environment. (D5.2, L5.2.1)

Question options:

A) 

Patches

B) 

Inventory

C) 

Baseline

D) 

Policy

Hide question 7 feedback

Correct. This is the definition of a baseline. 

**Question 8**

0 / 1 point

What is the most important aspect of security awareness/training? (D5.4, L5.4.1)

Question options:

A) 

Protecting assets

B) 

Maximizing business capabilities

C) 

Ensuring the confidentiality of data

D) 

Protecting health and human safety

Hide question 8 feedback

Incorrect. While protecting data is important, health and human safety are paramount. 

**Question 9**

1 / 1 point

Which entity is most likely to be tasked with monitoring and enforcing security policy? (D5.3, L5.3.1)

Question options:

A) 

The Human Resources office

B) 

The legal department

C) 

Regulators

D) 

The security office

Hide question 9 feedback

Correct. While the policy is dictated by senior management, the security office is often tasked with monitoring/enforcing it. 

**Question 10**

1 / 1 point

Which organizational policy is most likely to indicate which types of smartphones can be used to connect to the internal IT environment? (D5.3, L5.3.1)

Question options:

A) 

The CM policy (change management)

B) 

The password policy

C) 

The AUP (acceptable use policy)

D) 

The BYOD policy (bring your own device)

Hide question 10 feedback

Correct. The BYOD policy typically describes which devices can be used to process data and access networks belonging to the organization. 

![Happy face](https://learn.isc2.org/d2l/img/0/Quizzes.Main.actFeedbackHappy.svg?v=20.23.2.18529 "Happy face")

**Congratulations, you passed the quiz!**

You've achieved an overall grade of 70% or higher and completed this activity.