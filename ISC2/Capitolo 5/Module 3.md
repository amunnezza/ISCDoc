# Module 3: Understand Best Practice Security Policies

Domain D5.3, D5.3.1, D5.3.2, D5.3.3, D5.3.4, D5.3.5, D5.3.6

#### Module Objective

-   L5.3.1 Explain the application of common security policies.

An organization’s security policies define what “security” means to that organization, which in almost all cases reflects the tradeoff between security, operability, affordability and potential risk impacts. Security policies express or impose behavioral or other constraints on the system and its use. Well-designed systems operating within these constraints should reduce the potential of security breaches to an acceptable level. 

>[!Security governance]+
(The entirety of the policies, roles, and processes the organization uses to make security decisions in an organization.) 

that does not align properly with organizational goals can lead to implementation of security policies and decisions that unnecessarily inhibit productivity, impose undue costs and hinder strategic intent.
Video **SecPolicy.mkv**


_Manny_: What kind of policies can organizations establish to help their employees or members protect their data? 
_Tasha_: Policies can include password requirements, limits on personal devices, and all kinds of other policies to ensure privacy and security. In this module, we'll explore the most common security policies found in organizations and identify some components of these policies
****
# Common Security Policies

All policies must support any regulatory and contractual obligations of the organization.  Sometimes it can be challenging to ensure the policy encompasses all requirements while remaining simple enough for users to understand. 

Here are six common security-related policies that exist in most organizations.

_Click on each tab to learn more._  

**Data Handling Policy**

Appropriate use of data: This aspect of the policy defines whether data is for use within the company, is restricted for use by only certain roles or can be made public to anyone outside the organization. In addition, some data has associated legal usage definitions. The organization’s policy should spell out any such restrictions or refer to the legal definitions as required. Proper data classification also helps the organization comply with pertinent laws and regulations. For example, classifying credit card data as confidential can help ensure compliance with the PCI DSS. One of the requirements of this standard is to encrypt credit card information. Data owners who correctly defined the encryption aspect of their organization’s data classification policy will require that the data be encrypted according to the specifications defined in this standard.

**Password Policy**
Every organization should have a password policy in place that defines expectations of systems and users. The password policy should describe senior leadership's commitment to ensuring secure access to data, outline any standards that the organization has selected for password formulation, and identify who is designated to enforce and validate the policy.

**Acceptable Use Policy (AUP)**
The acceptable use policy (AUP) defines acceptable use of the organization’s network and computer systems and can help protect the organization from legal action. It should detail the appropriate and approved usage of the organization’s assets, including the IT environment, devices and data. Each employee (or anyone having access to the organization’s assets) should be required to sign a copy of the AUP, preferably in the presence of another employee of the organization, and both parties should keep a copy of the signed AUP. 

Policy aspects commonly included in AUPs: 

-   Data access
-   System access
-   Data disclosure
-   Passwords
-   Data retention
-   Internet usage
-   Company device usage

**Bring Your Own Device (BYOD) Policy**
An organization may allow workers to acquire equipment of their choosing and use personally owned equipment for business (and personal) use. This is sometimes called bring your own device (BYOD). Another option is to present the teleworker or employee with a list of approved equipment and require the employee to select one of the products on the trusted list. 

Letting employees choose the device that is most comfortable for them may be good for employee morale, but it presents additional challenges for the security professional because it means the organization loses some control over standardization and privacy. If employees are allowed to use their phones and laptops for both personal and business use, this can pose a challenge if, for example, the device has to be examined for a forensic audit. It can be hard to ensure that the device is configured securely and does not have any backdoors or other vulnerabilities that could be used to access organizational data or systems. 

All employees must read and agree to adhere to this policy before any access to the systems, network and/or data is allowed. If and when the workforce grows, so too will the problems with BYOD. Certainly, the appropriate tools are going to be necessary to manage the use of and security around BYOD devices and usage. The organization needs to establish clear user expectations and set the appropriate business rules.

**Privacy Policy**
Often, personnel have access to personally identifiable information (PII) (also referred to as electronic protected health information (_ePHI_) in the health industry). It is imperative that the organization documents that the personnel understand and acknowledge the organization’s policies and procedures for handling of that type of information and are made aware of the legal repercussions of handling such sensitive data. This type of documentation is similar to the AUP but is specific to privacy-related data. 

The organization’s privacy policy should stipulate which information is considered PII/ePHI, the appropriate handling procedures and mechanisms used by the organization, how the user is expected to perform in accordance with the stated policy and procedures, any enforcement mechanisms and punitive measures for failure to comply as well as references to applicable regulations and legislation to which the organization is subject. This can include national and international laws, such as the GDPR in the EU and Personal Information Protection and Electronic Documents Act (PIPEDA) in Canada; laws for specific industries in certain countries such as HIPAA and Gramm–Leach–Bliley Act (GLBA); or local laws in which the organization operates. 

The organization should also create a public document that explains how private information is used, both internally and externally. For example, it may be required that a medical provider present patients with a description of how the provider will protect their information (or a reference to where they can find this description, such as the provider’s website).

**Change Management Policy**
Change management is the discipline of transitioning from the current state to a future state. It consists of three major activities: deciding to change, making the change, and confirming that the change has been correctly accomplished. Change management focuses on making the decision to change and results in the approvals to systems support teams, developers and end users to start making the directed alterations.  

Throughout the system life cycle, changes made to the system, its individual components and its operating environment all have the capability to introduce new vulnerabilities and thus undermine the security of the enterprise. Change management requires a process to implement the necessary changes so they do not adversely affect business operations.
****
# Common Security Policies Deeper Dive

Policies will be set according to the needs of the organization and its vision and mission. Each of these policies should have a penalty or a consequence attached in case of noncompliance. The first time may be a warning; the next might be a forced leave of absence or suspension without pay, and a critical violation could even result in an employee’s termination. All of this should be outlined clearly during onboarding, particularly for information security personnel. It should be made clear who is responsible for enforcing these policies, and the employee must sign off on them and have documentation saying they have done so. This process could even include a few questions in a survey or quiz to confirm that the employees truly understand the policy. These policies are part of the baseline security posture of any organization. Any security or data handling procedures should be backed up by the appropriate policies.
****
# Keith Writes a Password Policy

video: KeithWrites.mkv

Tasha: Sandra's having trouble logging on to her work account. 
Sandra: Why won't it take my password? 
Keith: Are you still using your old password? 
Sandra: Yeah, it's what I always use. 
Keith: Oh, that’s why. You need a new password. The old password expires after 12 weeks. 
Sandra: Why did you do that? I like my password just the way it was. 
Keith: It's safer. Didn't you get my email I sent yesterday, or last week, or the one the week before that? 
Sandra: Hey, I thought it was for employees. I'm the owner. I'm not an employee. 
Keith: It's for everybody, including you. Let me show you how to reset your password. Sandra: Oh, you just do it for me. My password is ‘1234.’ 
Keith: Not anymore it isn't. We had to increase our requirements to help keep the bad guys out. And as the owner, your account is more valuable than the rest of the employees. New passwords have to have at least eight characters, upper and lower case, plus a number and a special character, like an exclamation point or a question mark. 
Sandra: Goodness – um, just make it ‘Keith1234.’ 
Keith: Yeah! 
Sandra: Question mark. 
Keith: Nobody’s going to guess that.
*****
# Change Management Components

The change management process includes the following components.
_Select each plus sign hotspot to learn more about each topic._

![[Change Management Components.png]]


#### **1 Request for Change**
##### Documentation
All of the major change management practices address a common set of core activities that start with a **request for change (RFC)** ( _def The first stage of change management, wherein a change in procedure or product is sought by a stakeholder.._) and move through various development and test stages until the change is released to the end users. From first to last, each step is subject to some form of formalized management and decision-making; each step produces accounting or log entries to document its results.

#### **2 Approval**
These processes typically include: Evaluating the RFCs for completeness, Assignment to the proper change authorization process based on risk and organizational practices, Stakeholder reviews, resource identification and allocation, Appropriate approvals or rejections, and Documentation of approval or rejection.

#### 3 Rollback
Depending upon the nature of the change, a variety of activities may need to be completed. These generally include: Scheduling the change, Testing the change, Verifying the rollback procedures, Implementing the change, Evaluating the change for proper and effective operation, and Documenting the change in the production environment. Rollback authority would generally be defined in the rollback plan, which might be immediate or scheduled as a subsequent change if monitoring of the change suggests inadequate performance.
*****
## video: Change Management Components in the Workplace

video: ChangeManage.mkv

Narrator: Change management happens in a cycle. There is no real stopping point; it is continuously going. This means that there must be continuous monitoring of that environment. So, if you or anyone should request a change, it needs to go through the appropriate approvals. The organization must be prepared for rollback if necessary, meaning that if that particular change did not work, we need to be able to roll back to the legacy system. While change management is an organization-wide process, it often falls on Information Security professionals to coordinate the effort and maybe to provide oversight and governance. Depending on the size of the organization, it may also fall under an IT or development area. In organizations that have a quality or risk management department, it would be a great fit in either of those areas too. The common theme is that change management acknowledges and incorporates input from the end users as well as all areas of IT, Development, Information Security and most importantly Management, to ensure that all changes are properly tested, approved and communicated prior to being implemented.
****
# Privacy Policy Knowledge Check

True or False? A privacy policy protects PII/ePHI from disclosure? (D5, L5.3.1) 

 True

 False

Check Answer

Correct answer: **True**

It’s true. A privacy policy documents how the organization’s personnel will handle personally identifiable information (PII), which is also referred to as electronic protected health information [ePHI] in the health industry, to ensure that it complies with any relevant national and international laws, such as the GDPR in the EU and Personal Information Protection and Electronic Documents Act (PIPEDA) in Canada; laws for specific industries in certain countries such as HIPAA and Gramm–Leach–Bliley Act (GLBA) in the U.S.; or local laws in which the organization operates.
****
# Change Management Policy Knowledge Check

For what purpose is a process required with a change management policy? (D5, L5.3.1) 

A. To define the standards for using the organization’s network and computer systems.
Incorrect. An acceptable use policy (AUP) defines acceptable use of the organization’s network, not a change management policy.

B. To help protect the organization in the event it faces legal action.
Incorrect. The acceptable use, privacy, BOYD and data handling policies help to protect the organization from legal action.

C. To establish the appropriate use of the organization’s data.
Incorrect. The data handling policy defines whether data is for use within the company, is restricted for use by only certain roles or can be made public to anyone outside the organization.

D. To ensure that systems changes are done without adversely affecting business operations.
**Correct**. Change management requires a process to implement necessary changes so they do not adversely affect business operations.
****
# Supporting Security Policies with Procedures - Video

video : SupportSecPolProcedure.mkv

Narrator: Different organizations will have different goals for their acceptable use policies. Some organizations encourage employees to make wide personal use of the organization’s IT assets, to improve morale and reduce interruptions between the user’s personal life and work. Some organizations encourage users to use organizational assets to perform personal educational tasks, as well—this way, the employee gets the benefit of the assets, and the organization gets a higher-trained and happier employee. Some organizations severely limit users' personal use of IT assets, in order to reduce risk within the organization. 
All security related policies should align with the organization’s risk tolerance while ensuring that regulatory requirements are met. An organization that does not store confidential data on a laptop or workstation is likely to be more relaxed in their acceptable use policy, while a healthcare facility, research institution or defense contractor may be much stricter, as they have data that can be potentially devastating if compromised.

FINE MODULE 3
