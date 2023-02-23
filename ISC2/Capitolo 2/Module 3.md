# Module 3: Understand Disaster Recovery (DR)

Domain D2.2, D2.2.1, D2.2.2, D2.2.3

#### Module Objective

-   L2.3.1 Identify the components of disaster recovery.

[Download Transcripts](https://learn.isc2.org/d2l/common/dialogs/quickLink/quickLink.d2l?ou=9238&type=coursefile&fileId=build%2fchapter_02%2ftranscripts%2fChapter%202%20Module%203%20Overview.pdf)

Manny: No matter how good the incident response and business continuity plans are, it seems likely that some lasting damage is going to be done. Some data is going to be lost or some services delayed. How do we get things back to normal? Tasha: That's where disaster recovery comes in. It picks up where business continuity left off. We discussed in the last module that business continuity is about maintaining critical business functions. These functions often rely on IT systems and communications. Disaster recovery planning is about restoring IT and communications back to full operation after a disruption, which we'll learn more about in this module.

# The Goal of Disaster Recovery

In the Business Continuity module, the essential elements of business continuity planning were explored. [Disaster recovery](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_02/module_03/ch02-m03-The_Goal_of_Disaster_Recovery.html?d2lSessionVal=70NMBm6xPErmD3jEMoqC7TdMJ&ou=9541&d2l_body_type=3#) planning steps in where BC leaves off. When a disaster strikes or an interruption of business activities occurs, the [Disaster recovery plan (DRP)](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_02/module_03/ch02-m03-The_Goal_of_Disaster_Recovery.html?d2lSessionVal=70NMBm6xPErmD3jEMoqC7TdMJ&ou=9541&d2l_body_type=3#) guides the actions of emergency response personnel until the end goal is reached—which is to see the business restored to full last-known reliable operations.

Disaster recovery refers specifically to restoring the information technology and communications services and systems needed by an organization, both during the period of disruption caused by any event and during restoration of normal services. The recovery of a business function may be done independently of the recovery of IT and communications services; however, the recovery of IT is often crucial to the recovery and sustainment of business operations. Whereas business continuity planning is about maintaining critical business functions, disaster recovery planning is about restoring IT and communications back to full operations after a disruption.




# Disaster Recovery in the Real World

We need to make sure that an organization’s critical systems are formally identified and have backups that are regularly tested. Sometimes an incident is not recognized or detected until days or months later.  

Click each plus sign on the image for examples of disaster recovery in the real world.

### Primo
At a hospital in Los Angeles, it took 260 days (about 8 and a half months) to discover that there was a compromise. In this case, the hospital could not return to doing business by using the last backup because it was riddled with a time-based malware that would corrupt all the data on the system as soon as it was restored. The hospital needed to go back nearly a year prior to discovering the incident to restore the entire system, and then restore the remaining data piece-by-piece to avoid reinfection. This scenario highlights the need for multiple levels of backup and retention periods to address the needs of the organization.

### Secondo
Complex systems can often store valuable information across several servers. While at its most basic level, disaster recovery plans include backing up data at a server level, it is also necessary to consider the database itself, as well as any dependencies on other systems. In this more complex scenario, data is entered by users into one system and database and is then distributed to other systems. This is common in large enterprises where multiple systems need to talk to each other to maintain common data. In another hospital example, the radiology department used a different system than the laboratory. In this case, a separate routine copied the patient data from the registration system to the laboratory and the radiology systems, which technically use separate databases. It is important to understand the flow of data and the intricate dependencies of one system on another to properly document and implement a disaster recovery plan that will be successful when it is needed.

# Components of a Disaster Recovery Plan

Depending on the size of the organization and the number of people involved in the DRP effort, organizations often maintain multiple types of plan documents, intended for different audiences. The following list includes various types of documents worth considering:

-   Executive summary providing a high-level overview of the plan
-   Department-specific plans
-   Technical guides for IT personnel responsible for implementing and maintaining critical backup systems
-   Full copies of the plan for critical disaster recovery team members
-   Checklists for certain individuals:

-   Critical disaster recovery team members will have checklists to help guide their actions amid the chaotic atmosphere of a disaster.
-   IT personnel will have technical guides helping them get the alternate sites up and running. 
-   Managers and public relations personnel will have simple-to-follow, high-level documents to help them communicate the issue accurately without requiring input from team members who are busy working on the recovery.

