# Module 1: Understand Access Control Concepts

Domain D3.1, D3.1.3, D3.1.5, D3.2, D3.2.1, D3.2.2, D3.2.5

#### Module Objective

-   L3.1.1 Relate access control concepts and processes given scenarios.
# Video Understand Access Control Concepts


Manny: In the last module, we covered all the planning that goes into incident response and disaster recovery. But how do security professionals protect information from falling into the wrong hands in the first place? Tasha: That's the topic of our next module. Information security professionals are like gatekeepers, controlling who gets access to which systems and data, why they get certain permissions or not, and how. Let's find out more about these access control concepts.


# What is Security Control?

A control is a safeguard or countermeasure designed to preserve Confidentiality, Integrity and Availability of data. This, of course, is the CIA Triad.  

Access control involves limiting what objects can be available to what subjects according to what rules. We will further define **==objects, subjects  and rules==** later in this chapter. For now, remember these three words, as they are the foundation upon which we will build. 

One brief example of a control is a firewall, which is included in a system or network to prevent something from the outside from coming in and disturbing or compromising the environment. The firewall can also prevent information on the inside from going out into the Web where it could be viewed or accessed by unauthorized individuals.

# Controls Overview

It can be argued that access controls are the heart of an information security program. Earlier in this course we looked at security principles through foundations of risk management, governance, incident response, business continuity and disaster recovery. But in the end, security all comes down to, “who can get access to organizational assets (buildings, data, systems, etc.) and what can they do when they get access?”

Access controls are not just about restricting access to information systems and data, but also about allowing access. It is about granting the appropriate level of access to authorized personnel and processes and denying access to unauthorized functions or individuals.

Access is based on three elements:  

_Click on each tab to learn more._

[Subjects](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_03/module_01/ch03_m01-Controls_Overview.html?d2lSessionVal=bsW1zJiTb77E7k71AldURfecn&ou=9541&d2l_body_type=3#list-1)[Objects](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_03/module_01/ch03_m01-Controls_Overview.html?d2lSessionVal=bsW1zJiTb77E7k71AldURfecn&ou=9541&d2l_body_type=3#list-2)[Rules](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_03/module_01/ch03_m01-Controls_Overview.html?d2lSessionVal=bsW1zJiTb77E7k71AldURfecn&ou=9541&d2l_body_type=3#list-3)

A [[PopUp3#^eb22cf|subject]] can be defined as any entity that requests access to our assets. The entity requesting access may be a user, a client, a process or a program, for example. A subject is the initiator of a request for service; therefore, a subject is referred to as “active.”

A **subject**:

-   Is a user, a process, a procedure, a client (or a server), a program, a device such as an endpoint, workstation, smartphone or removable storage device with onboard firmware.
-   Is active: It initiates a request for access to resources or services.
-   Requests a service from an object.
-   Should have a level of clearance (permissions) that relates to its ability to successfully access services or resources.

**object**

By definition, anything that a subject attempts to access is referred to as an  
> [!FAQ]-  Object  
> Passive information-related entity (e.g. devices, files, records, tables, processes, programs, domains) containing or receiving information. Access to an object (by subject) implies access to the information it contains. See subject.
> NIST SP800-53-R4

An object is a device, process, person, user, program, server, client or other entity that responds to a request for service. Whereas a subject is active in that it initiates a request for a service, an object is passive in that it takes no action until called upon by a subject. When requested, an object will respond to the request it receives, and if the request is wrong, the response will probably not be what the subject really wanted either.
Note that by definition, objects do not contain their own access control logic. Objects are passive, not active (in access control terms), and must be protected from unauthorized access by some other layers of functionality in the system, such as the integrated identity and access management system. An object has an owner, and the owner has the right to determine who or what should be allowed access to their object. Quite often the rules of access are recorded in a rule base or access control list.

An object:

-   Is a building, a computer, a file, a database, a printer or scanner, a server, a communications resource, a block of memory, an input/output port, a person, a software task, thread or process.
-   Is anything that provides service to a user.
-   Is passive.
-   Responds to a request.
-   May have a classification.


**Rule**
An access [[PopUp3#^d11d3e|Rule]] is an instruction developed to allow or deny access to an object by comparing the validated identity of the subject to an access control list. One example of a rule is a [[PopUp3#^firewall|firewall]] access control list. By default, firewalls deny access from any address to any address, on any port. For a firewall to be useful, however, it needs more rules. A rule might be added to allow access from the inside network to the outside network. Here we are describing a rule that allows access to the object “outside network” by the subject having the address “inside network.” In another example, when a user (subject) attempts to access a file (object), a rule validates the level of access, if any, the user should have to that file. To do this, the rule will contain or reference a set of attributes that define what level of access has been determined to be appropriate.

A rule can:

-   Compare multiple attributes to determine appropriate access.
-   Allow access to an object.
-   Define how much access is allowed.
-   Deny access to an object.
-   Apply time-based access.





# Controls and Risks

[Download Transcript](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_03/transcripts/Controls%20and%20Risks.pdf?_&d2lSessionVal=64z4ddVDcNlmubHwLpng93Gnv&ou=9541)
## video  Controls and Risks

Narrator: A control serves to reduce the risk to where it is within the risk tolerance of the individual or organization. A physical control would be a seat belt. An administrative control would be a law requiring the use of the seatbelt. Both of these serve to reduce the risk of driving to a degree that is acceptable to the driver and to society. Another non-technical example is that of a tall bookshelf. Since there is a risk of a tall bookshelf toppling over and possibly hurting someone, many local building codes or regulations require bookshelves to be secured to a wall using a strap or a bracket. In this case, the risk is the injury to people. A logical control is the building code, and the actual attachment of the shelf to the wall is the physical control. Both logical and physical controls work together to mitigate the risk.


# Controls Assessments

Risk reduction depends on the effectiveness of the control. It must apply to the current situation and adapt to a changing environment. 

Consider a scenario where part of an office building is being repurposed for use as a secure storage facility. Due to the previous use of the area, there are 5 doors which must be secured before confidential files can be stored there. When securing a physical location, there are several things to consider. To keep the information the most secure, it might be recommended to install biometric scanners on all doors. A site assessment will determine if all five doors need biometric scanners, or if only one or two doors need scanners. The remaining doors could be permanently secured, or if the budget permits, the doors could be removed and replaced with a permanent wall. Most importantly, the cost of implementing the controls must align with the value of what is being protected.  If multiple doors secured by biometric locks are not necessary, and the access to the area does not need to be audited, perhaps a simple deadbolt lock on all of the doors will provide the correct level of control.

# Defense in Depth

As you can see, we are not just looking at system access. We are looking at all access permissions including building access, access to server rooms, access to networks and applications and utilities. These are all implementations of access control and are part of a [[PopUp3#^9bfb75|LAYERED DEFENSE]] strategy, also known as [[PopUp3#^18d837|defense in depth]], developed by an organization.

Defense in depth describes an information security strategy that integrates people, technology and operations capabilities to establish variable barriers across multiple layers and missions of the organization. It applies multiple countermeasures in a layered fashion to fulfill security objectives. Defense in depth should be implemented to prevent or deter a cyberattack, but it cannot guarantee that an attack will not occur. 

A technical example of defense in depth, in which multiple layers of technical controls are implemented, is when a username and password are required for logging in to your account, followed by a code sent to your phone to verify your identity. This is a form of multi-factor authentication using methods on two layers, something you have and something you know. The combination of the two layers is much more difficult for an adversary to obtain than either of the authentication codes individually. 

Another example of multiple technical layers is when additional firewalls are used to separate untrusted networks with differing security requirements, such as the internet from trusted networks that house servers with sensitive data in the organization. When a company has information at multiple sensitivity levels, it might require the network traffic to be validated by rules on more than one firewall, with the most sensitive information being stored behind multiple firewalls.

![concentric circles with Assets at the center followed by Administrative Controls, Logical/Technical Controls, and with Physical Controls at the outer circle](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_03/assets/EDU-ELCC-70510-defense_in_depth-techart-v01.svg?_&d2lSessionVal=64z4ddVDcNlmubHwLpng93Gnv&ou=9541 "concentric circles with Assets at the center followed by Administrative Controls, Logical/Technical Controls, and with Physical Controls at the outer circle")

![[EDU-ELCC-70510-defense_in_depth-techart-v01.jpeg]]


For a non-technical example, consider the multiple layers of access required to get to the actual data in a data center. First, a lock on the door provides a physical barrier to access the data storage devices. Second, a technical access rule prevents access to the data via the network. Finally, a policy, or administrative control defines the rules that assign access to authorized individuals.

# Defense in Depth Practice
VIDEO Defense in Depth Practice

[Transcript]
Narrator: A data center might have multiple layers of defense. We would have administrative controls, such as policies and procedures. Then logical or technical controls, which include programming to limit access. There are also physical controls, which we sometimes forget about in our highly technical world. Regardless of how much we focus on cloud computing and virtualization, there is always a physical location where information is being stored or processed in a physical hard drive in a physical computer. Even in a data center in a large organization that provides cloud computing services, for example, there is still a physical aspect of information storage and processing.

# Principle of Least Privilege

The 
> [!Principle of Least Privilege]- PRINCIPLE OF LEAST PRIVILEGE
> The principle that users and programs should have only the minimum privilege necessary to complete their task. NIST SP 800-179 


Is a standard of permitting only minimum access necessary for users or programs to fulfill their function. Users are provided access only to the systems and programs they need to perform their specific job or tasks.

##VIDEO PRINCIPLEOFLEATPRIVILEGE.MKV

TRANSCRIPT
Tasha: Gabriela is a recent new hire at JavaSip, and she's reached out to Nate for some help. Gabriela: Hey Nate? Nate: Yep? Gabriela: I accidentally submitted my timecard already, and I can't get into the payroll system to fix it. Nate: Well, of course you can’t get into the system. Only the manager, that's me, can get into the payroll system. Otherwise, we'd risk everyone giving themselves raises, not to mention having access to other employees' confidential information. Here, let me show you. There it is. Gabriela: Oh. Yeah. Nate: All good. Gabriela: Thanks! Nate: Welcome. Tasha: Nate explains to Gabriela that her access to the system is limited by her role. She doesn't have the proper permissions to make changes to her timecard, just to complete and submit it. That's all she needs to do in her position, so she is restricted from other functions in the system, but he's happy to help and reassures Gabriela that he will make the necessary changes.

# Examples of Least Privilege

To preserve the confidentiality of information and ensure that it is only available to personnel who are authorized to see it, we use privileged access management, which is based on the principle of least privilege. That means each user is granted access only to the items they need and nothing further.  

For example, only individuals working in billing will be allowed to view consumer financial data, and even fewer individuals will have the authority to change or delete that data. This maintains confidentiality and integrity while also allowing availability by providing administrative access with an appropriate password or sign-on that proves the user has the appropriate permissions to access that data.  

Sometimes it is necessary to allow users to access the information via a temporary or limited access, for instance, for a specific time period or just within normal business hours. Or access rules can limit the fields that the individuals can have access to. One example is a healthcare environment. Some workers might have access to patient data but not their medical data. Individual doctors might have access only to data related to their own patients. In some cases, this is regulated by law, such as HIPAA in the United States, and by specific privacy laws in other countries. 

Systems often monitor access to private information, and if logs indicate that someone has attempted to access a database without the proper permissions, that will automatically trigger an alarm. The security administrator will then record the incident and alert the appropriate people to take action.  

The more critical information a person has access to, the greater the security should be around that access. They should definitely have multi-factor authentication, for instance.

# Privileged Access Management

Privileged access management provides the first and perhaps most familiar use case. Consider a human user identity that is granted various create, read, update, and delete privileges on a database. Without privileged access management, the system’s access control would have those privileges assigned to the administrative user in a static way, effectively “on” 24 hours a day, every day. Security would be dependent upon the login process to prevent misuse of that identity. Just-in-time privileged access management, by contrast, includes role-based specific subsets of privileges that only become active in real time when the identity is requesting the use of a resource or service. 

Consider this scenario explaining why privileged access management is important:

_ABC, Inc., has a small IT department that is responsible for_
>[!user provisioning]- User provisioning
>The process of creating, mantaining and deactivating user identities on a system. 
> 

_and administering systems. To save time, the IT department employees added their IDs to the Domain Admins group, effectively giving them access to everything within the Windows server and workstation environment. While reviewing an invoice that was received via email, they opened an email that had a malicious attachment that initiated a_
>[!ransomware]- ransomware
>a type of malicious software that locks the computer screen of files, thus preventing or limiting a user from accessing their system and data until money is paid.

_attack. Since they are using Domain Admin privileges, the ransomware was able to_ 
>[!encrypt]- encrypt 
>to protect private information by putting it into a form that can only be read by people who have permission to do so. 

_all the files on all servers and workstations. A privileged access management solution could limit the damage done by this ransomware if the administrator privileges are only used when performing a function requiring that level of access. Routine operations, such as daily email tasks, are done without a higher level of access._

# Privileged Accounts

>[!Privileged accounts]- Privileged accounts
>An information system account whith approved authorization of a privileged user. NIST SOP 800-53 REV. 4

are those with permissions beyond those of normal users, such as managers and administrators. 

Broadly speaking, these accounts have elevated privileges and are used by many different classes of users, including: 

-   Systems administrators, who have the principal responsibilities for operating systems, applications deployment and performance management. 
-   Help desk or IT support staff, who often need to view or manipulate endpoints, servers and applications platforms by using privileged or restricted operations. 
-   Security analysts, who may require rapid access to the entire IT infrastructure, systems, endpoints and data environment of the organization. 

Other classes of privileged user accounts may be created on a per-client or per-project basis, to allow a member of that project or client service team to have greater control over data and applications. 

These few examples indicate that organizations often need to delegate the capability to manage and protect information assets to various managerial, supervisory, support or leadership people, with differing levels of authority and responsibility. This delegation, of course, should be contingent upon trustworthiness, since misuse or abuse of these privileges could lead to harm for the organization and its stakeholders. 

Typical measures used for moderating the potential for elevated risks from misuse or abuse of privileged accounts include the following: 

-   More extensive and detailed 
  >[!logging]- Logging
  >Collecting and storing user activity in a log, which is a record of the events occurring within an organization's systems and networks
- 
- than regular user accounts. The record of privileged actions is vitally important, as both a deterrent (for privileged account holders that might be tempted to engage in untoward activity) and an administrative control (the logs can be
  >[!audited]- Audited
  >Indipendent review and examinations of records and activities to assess the adequacy of system controls, to ensure compliance with established policies and operational procedures. NIST SP 1800-15B
 
 and reviewed to detect and respond to malicious activity). 
-   More stringent access control than regular user accounts. As we will see emphasized in this course, even nonprivileged users should be required to use MFA methods to gain access to organizational systems and networks. Privileged users—or more accurately, highly trusted users with access to privileged accounts—should be required to go through additional or more rigorous authentication prior to those privileges. Just-in-time identity should also be considered as a way to restrict the use of these privileges to specific tasks and the times in which the user is executing them. 
-   Deeper trust verification than regular user accounts. Privileged account holders should be subject to more detailed background checks, stricter nondisclosure agreements and acceptable use policies, and be willing to be subject to financial investigation. Periodic or event-triggered updates to these background checks may also be in order, depending on the nature of the organization’s activities and the risks it faces. 
-   More auditing than regular user accounts. Privileged account activity should be monitored and audited at a greater rate and extent than regular usage. 

_Click on the plus sign + below to learn more._

## Explore Privileged Access Management Further

Let's consider the Help Desk role. In order to provide the level of service customers demand, it may be necessary for your Help Desk personnel to reset passwords and unlock user accounts.  In a Windows environment, this typically requires “domain admin” privileges.  However, these two permissions can be granted alone, giving the Help Desk personnel a way to reset passwords without giving them access to everything in the Windows domain, such as adding new users or changing a user’s information. These two actions should be logged and audited on a regular basis to ensure that any password resets were requested by the end user. This can be done by automatically generating a daily list of password resets to be compared to Help Desk tickets. This scenario allows the Help Desk personnel to resolve password-related issues on the first call while doing so in a safe and secure manner.

# Segregation of Duties 

A core element of authorization is the principle of 
>[!segregation of duties]- segregation of duties
>The practice of ensuring that an organizational process cannot be completed by a single person: forces collusion as a means to reduce insider threats. Also known as Separation of Duties

(also known as separation of duties). Segregation of duties is based on the security practice that no one person should control an entire high-risk transaction from start to finish. Segregation of duties breaks the transaction into separate parts and requires a different person to execute each part of the transaction. For example, an employee may submit an invoice for payment to a vendor (or for reimbursement to themselves), but it must be approved by a manager prior to payment; in another instance, almost anyone may submit a proposal for a change to a system configuration, but the request must go through technical and management review and gain approval, before it can be implemented.

These steps can prevent fraud or detect an error in the process before implementation. It could be that the same employee might be authorized to originally submit invoices regarding one set of activities, but not approve them, and yet also have approval authority but not the right to submit invoices on another. It is possible, of course, that two individuals can willfully work together to bypass the segregation of duties, so that they could jointly commit fraud. This is called collusion.

Another implementation of segregation of duties is dual control. This would apply at a bank where there are two separate combination locks on the door of the vault. Some personnel know one of the combinations and some know the other, but no one person knows both combinations. Two people must work together to open the vault; thus, the vault is under dual control. 

## Two-Person Integrity 

The two-person rule is a security strategy that requires a minimum of two people to be in an area together, making it impossible for a person to be in the area alone. Many access control systems prevent an individual cardholder from entering a selected high-security area unless accompanied by at least one other person. Use of the two-person rule can help reduce 
>[!insider threats]- Insider threats
>An entity with authorized access that has the potential to harm an information system through 

to critical areas by requiring at least two individuals to be present at any time. It is also used for life safety within a security area; if one person has a medical emergency, there will be assistance present.

# Authorized Versus Unauthorized Personnel

Subjects are authorized access to objects after they have been authenticated. Remember from earlier sections that authentication is confirming the identity of the subject. Once a subject has been authenticated, the system checks its authorization to see if it is allowed to complete the action it is attempting. This is usually done via a security matrix accessed by the system controlling the access, based on pre-approved levels. For example, when a person presents an ID badge to the data center door, the system checks the ID number, compares that to a security matrix within the system, and unlocks the door if the ID is authorized. If the ID is not authorized to unlock the door, it will remain locked. In another example, a user attempts to delete a file. The file system checks the permissions to see if the user is authorized to delete the file. If the user is authorized, the file is deleted. If the user is not authorized, an error message is displayed, and the file is left untouched.


# How Users Are Provisioned

Other situations that call for provisioning new user accounts or changing privileges include: 

-   **A new employee**—When a new employee is hired, the hiring manager sends a request to the security administrator to create a new user ID. This request authorizes creation of the new ID and provides instructions on appropriate access levels. Additional authorization may be required by company policy for elevated permissions. 
-   **Change of position**—When an employee has been promoted, their permissions and access rights might change as defined by the new role, which will dictate any added privileges and updates to access. At the same time, any access that is no longer needed in the new job will be removed. 
-   **Separation of employment**—When employees leave the company, depending on company policy and procedures, their accounts must be disabled after the termination date and time. It is recommended that accounts be disabled for a period before they are deleted to preserve the integrity of any audit trails or files that may be owned by the user. Since the account will no longer be used, it should be removed from any security roles or additional access profiles. This protects the company, so the separated employee is unable to access company data after separation, and it also protects them because their account cannot be used by others to access data.

_**NOTE:** Upon hiring or changing roles, a best practice is to not copy user profiles to new users, because this promotes “permission or privilege creep.” For example, if an employee is given additional access to complete a task and that access is not removed when the task is completed, and then that user’s profile is copied to create a new user ID, the new ID is created with more permissions than are needed to complete their functions. It is recommended that standard roles are established, and new users are created based on those standards rather than an actual user._

# VIDEO How user are provisioned.mkv


[Download Transcript](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_03/transcripts/How%20Users%20are%20Provisioned.pdf?_&d2lSessionVal=wBf5RF153cET3tOd27DI4UTS8&ou=9541)
Tasha: Whether a user is authorized or unauthorized depends on their user provisioning, which is an identity management process for creating and managing access to resources and information systems. Manny: While we usually think of user provisioning as creating new accounts, there are several different situations which require action by a security administrator who is responsible for provisioning user accounts. Tasha: In fact, Susan finds herself in a situation that requires changes to a user’s provisioning. Let's check in with her as she notifies the security administrator of this change. Susan is talking to her securityadministrator. Susan: One of my employees will be taking a temporary leave of absence. Dimitra, she’s going to be taking a sabbaticalfrom work and she’s not going to need access to the systems Manny: Since Dimitra will not be accessing the systems, the security admin recommends disabling her accounts while she is not at work. This reduces the risk that her account could be used by an unauthorized person while she is on leave. He tells Susan to make the request, and then, according to the company policy and procedures, he will disable Dimitra's login account, so she is not allowed to log in to the company systems while out on leave. Susan: So, will this make things complicated when Dimitra returns to work? Oh, I see. Even though the account is disabled, but not otherwise modified, it will be easy to reactivate it once she returns. That's great news, because I’m going to need her up and running as soon as she gets back.

# Roles and Permissions

  

Compare and Contrast a Regular User Account Permissions to a Privileged User Account Permissions.

Which role would get Regular Account permissions? (Select all that would apply.)

 Part-time Employee

 Remote Employee

 This option is incorrect. Chief Information Security Officer

 This option is incorrect. Network Admin

 This option is incorrect. System Admin

 Full-time Employee

 Temporary Employee

 Manager/Team Lead

Check Answer

The  indicates the correct selection.


# Privileged Access Management

Compare and Contrast a Regular User Account to a Privileged User Account.

A Privileged User Account: (Select all that would apply.)

Has access to interact directly with servers and other infrastructure devices.

 This option is incorrect. Has access to log on only to authorized workstations.

 This option is incorrect. Is most likely to have read-only access to a database.

 This option is incorrect. Has access levels that are typically needed for daily business operations.

 This option is incorrect. Has the lowest level of logging associated with actions.

Should require the use of MFA.

Uses the most stringent access control.

Has the highest level of logging associated with actions.

Often has the ability to create users and assign permissions.

Check Answer

The  indicates the correct selection.

# The Benefit of Multiple Controls

## VIDEO # The Benefit of Multiple Controls.MKV


[Download Transcript]
Narrator: A control is a safeguard or countermeasure designed to preserve Confidentiality, Integrity and Availability of data. We also discussed defense-in-depth as an implementation of multiple technical controls. Now, we will look at a scenario that uses multiple controls across the spectrum, including physical, technical and administrative controls. Payroll is one area in nearly every organization that requires multiple levels of controls to ensure money is not mishandled. Most will agree that just a single control is too risky, so multiple controls are often implemented. To prevent payroll personnel from creating a fictional employee and processing a check for that employee, a logical (or technical) control is to ensure that a person who processes payroll is not able to create a new employee record AND process the check print file. A physical control that helps reinforce that technical control is to ensure the actual paper media that checks are printed on is secured in a place that is not accessible to the person processing payroll. Both of these controls can be further enforced by creating an administrative control (or policy) that regularly audits the technical and physical controls by reviewing new employees added to the system and by logging and verifying the number on physical checks. Small and medium businesses have a particular challenge when it comes to technical controls, as they often do not have sufficient personnel to separate the duties within the payroll system. In this case, it may become necessary to implement only physical and logical controls that align with the business needs.