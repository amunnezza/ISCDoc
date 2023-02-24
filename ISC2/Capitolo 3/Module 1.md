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

A [subject]() can be defined as any entity that requests access to our assets. The entity requesting access may be a user, a client, a process or a program, for example. A subject is the initiator of a request for service; therefore, a subject is referred to as “active.”

A **subject**:

-   Is a user, a process, a procedure, a client (or a server), a program, a device such as an endpoint, workstation, smartphone or removable storage device with onboard firmware.
-   Is active: It initiates a request for access to resources or services.
-   Requests a service from an object.
-   Should have a level of clearance (permissions) that relates to its ability to successfully access services or resources.

**object**

By definition, anything that a subject attempts to access is referred to as an [object](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_03/module_01/ch03_m01-Controls_Overview.html?d2lSessionVal=99O2UR5qjY9IQl18VvNmhOp0S&ou=9541&d2l_body_type=3#). An object is a device, process, person, user, program, server, client or other entity that responds to a request for service. Whereas a subject is active in that it initiates a request for a service, an object is passive in that it takes no action until called upon by a subject. When requested, an object will respond to the request it receives, and if the request is wrong, the response will probably not be what the subject really wanted either.

Note that by definition, objects do not contain their own access control logic. Objects are passive, not active (in access control terms), and must be protected from unauthorized access by some other layers of functionality in the system, such as the integrated identity and access management system. An object has an owner, and the owner has the right to determine who or what should be allowed access to their object. Quite often the rules of access are recorded in a rule base or access control list.

An object:

-   Is a building, a computer, a file, a database, a printer or scanner, a server, a communications resource, a block of memory, an input/output port, a person, a software task, thread or process.
-   Is anything that provides service to a user.
-   Is passive.
-   Responds to a request.
-   May have a classification.


**Rule**
An access [[PopUp#^d11d3e|Rule]] is an instruction developed to allow or deny access to an object by comparing the validated identity of the subject to an access control list. One example of a rule is a [[PopUp#^firewall|firewall]] access control list. By default, firewalls deny access from any address to any address, on any port. For a firewall to be useful, however, it needs more rules. A rule might be added to allow access from the inside network to the outside network. Here we are describing a rule that allows access to the object “outside network” by the subject having the address “inside network.” In another example, when a user (subject) attempts to access a file (object), a rule validates the level of access, if any, the user should have to that file. To do this, the rule will contain or reference a set of attributes that define what level of access has been determined to be appropriate.

A rule can:

-   Compare multiple attributes to determine appropriate access.
-   Allow access to an object.
-   Define how much access is allowed.
-   Deny access to an object.
-   Apply time-based access.


















 