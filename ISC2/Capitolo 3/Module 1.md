# Module 1: Understand Access Control Concepts

Domain D3.1, D3.1.3, D3.1.5, D3.2, D3.2.1, D3.2.2, D3.2.5

#### Module Objective

-   L3.1.1 Relate access control concepts and processes given scenarios.
# scaricare Video

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

By definition, anything that a subject attempts to access is referred to as an [[PopUp3#^4aeafa|object]]. An object is a device, process, person, user, program, server, client or other entity that responds to a request for service. Whereas a subject is active in that it initiates a request for a service, an object is passive in that it takes no action until called upon by a subject. When requested, an object will respond to the request it receives, and if the request is wrong, the response will probably not be what the subject really wanted either.

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
##scarica video

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

For a non-technical example, consider the multiple layers of access required to get to the actual data in a data center. First, a lock on the door provides a physical barrier to access the data storage devices. Second, a technical access rule prevents access to the data via the network. Finally, a policy, or administrative control defines the rules that assign access to authorized individuals.

# Defense in Depth Practice
DOWNLOAD VIDEO

[Transcript]
Narrator: A data center might have multiple layers of defense. We would have administrative controls, such as policies and procedures. Then logical or technical controls, which include programming to limit access. There are also physical controls, which we sometimes forget about in our highly technical world. Regardless of how much we focus on cloud computing and virtualization, there is always a physical location where information is being stored or processed in a physical hard drive in a physical computer. Even in a data center in a large organization that provides cloud computing services, for example, there is still a physical aspect of information storage and processing.











 