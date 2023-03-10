# Module 3: Understand Disaster Recovery (DR)

Domain D2.2, D2.2.1, D2.2.2, D2.2.3

#### Module Objective

-   L2.3.1 Identify the components of disaster recovery.

[Download Transcripts](https://learn.isc2.org/d2l/common/dialogs/quickLink/quickLink.d2l?ou=9238&type=coursefile&fileId=build%2fchapter_02%2ftranscripts%2fChapter%202%20Module%203%20Overview.pdf)

Manny: No matter how good the incident response and business continuity plans are, it seems likely that some lasting damage is going to be done. Some data is going to be lost or some services delayed. How do we get things back to normal? Tasha: That's where disaster recovery comes in. It picks up where business continuity left off. We discussed in the last module that business continuity is about maintaining critical business functions. These functions often rely on IT systems and communications. Disaster recovery planning is about restoring IT and communications back to full operation after a disruption, which we'll learn more about in this module.
****
# The Goal of Disaster Recovery

In the Business Continuity module, the essential elements of business continuity planning were explored. 
>[!Disaster recovery]-
>In information systems terms, the activities necessary to restore IT and communications services to an organization during and after an outage, disruption or disturbance of any kind or scale.

planning steps in where BC leaves off. When a disaster strikes or an interruption of business activities occurs, the **Disaster recovery plan (DRP)** (_def:  The processes, policies and procedures related to preparing for recovery or continuation of an organization's critical business functions, technology infrastructure, systems and applications after the organization experiences a disaster. A disaster is when an organization’s critical business function(s) cannot be performed at an acceptable level within a predetermined period following a disruption._ ) guides the actions of emergency response personnel until the end goal is reached—which is to see the business restored to full last-known reliable operations.

Disaster recovery refers specifically to restoring the information technology and communications services and systems needed by an organization, both during the period of disruption caused by any event and during restoration of normal services. The recovery of a business function may be done independently of the recovery of IT and communications services; however, the recovery of IT is often crucial to the recovery and sustainment of business operations. Whereas business continuity planning is about maintaining critical business functions, disaster recovery planning is about restoring IT and communications back to full operations after a disruption.
****
# Disaster Recovery in the Real World

We need to make sure that an organization’s critical systems are formally identified and have backups that are regularly tested. Sometimes an incident is not recognized or detected until days or months later.  

Click each plus sign on the image for examples of disaster recovery in the real world.

### Primo
At a hospital in Los Angeles, it took 260 days (about 8 and a half months) to discover that there was a compromise. In this case, the hospital could not return to doing business by using the last backup because it was riddled with a time-based malware that would corrupt all the data on the system as soon as it was restored. The hospital needed to go back nearly a year prior to discovering the incident to restore the entire system, and then restore the remaining data piece-by-piece to avoid reinfection. This scenario highlights the need for multiple levels of backup and retention periods to address the needs of the organization.

### Secondo
Complex systems can often store valuable information across several servers. While at its most basic level, disaster recovery plans include backing up data at a server level, it is also necessary to consider the database itself, as well as any dependencies on other systems. In this more complex scenario, data is entered by users into one system and database and is then distributed to other systems. This is common in large enterprises where multiple systems need to talk to each other to maintain common data. In another hospital example, the radiology department used a different system than the laboratory. In this case, a separate routine copied the patient data from the registration system to the laboratory and the radiology systems, which technically use separate databases. It is important to understand the flow of data and the intricate dependencies of one system on another to properly document and implement a disaster recovery plan that will be successful when it is needed.
****
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

# Disaster Recovery in Action

File video DisasterRecoveryAction.mkv
Transcript:
Narrator: An example of disaster recovery in action is the use of system backups. The timeline in this image looks backward in time from the moment of incident detection (on the right) as a way of identifying the amount of work that will be lost by reloading from a backup. Transaction processing events (the triangles) and some backup events (shown as database symbols) have been numbered as events 1 through 21 from left to right along the timeline. The green transactions (events 1 through 14) are ones that were fully processed prior to the intrusion or the start of the incident. Presumably, and if antivirus and other systems are working correctly, this may be a safe assumption. These transactions were not exposed to possible loss of integrity, authenticity, privacy, or any other required security attributes. The database symbols shown in gray (events 2, 5, 9, and 13—all prior to the event) represent some form of system and data backup that may have captured the changes to the system as a result of properly completing the green transactions. It is events 15 through 21, however, that are in doubt. They may be okay, or they may represent a lack of integrity if the data was compromised. The database backup symbols in orange, between the time of the incidence occurrence and it's being detected, are clearly in doubt as to their integrity or safety. They may contain bogus, corrupted data or they may even contain malware in a variety of forms. Moving backward in time from the detection of the incident, it's not until we get to that right most gray database symbol—event 13 the backup just before the incident occurs—that we have our last clean, trustworthy backup. Three sets of work that were lost since the incident started to occur can be identified: all transactions or changes prior to that last good backup that were not part of that backup—if it was an incremental or partial backup and not a full backup—events 15, 17 through 19 and 21; all transactions and other changes processed or attempted from that backup forward in time until after the incident was detected, not started to occur; and all transactions changes, etc. that would normally have been processed from the time the incident was detected until the system was fully operational again, but were not able to be processed at all due to the disruption.


# When Lightning Strikes

File video: WhenLightingStrike.mkv

Transcript
Manny: During a bad lightning storm last night, JavaSip experienced a power surge that damaged the company computer. Sandra: (Groaning) Oh, I can't believe it. The power surge killed the computer. It won't even turn on. Now what are we going to do? Keith: Seems like we need a new computer. Sandra: Well, that's the least of our worries. What about everything that's on the computer? Everything we need to run this coffee shop is on the computer. Keith: It's okay, Mom. Remember? As part of our disaster recovery plan, Nate and I have been backing up the system every night after we close. Sandra: Are you serious? You have everything backed up? Keith: Everything. It's all on an external hard drive that we take home every night after we close. Sandra: (Laughing) Thank goodness. I'm so proud of you. See, we need you here at JavaSip. Keith: Aw, thanks, Mom. Glad I can help. It's just too bad I couldn't predict a power surge that'd impact the business like this. But look, you go get a new computer and get a surge protector while you're at it. Sandra: I agree. We do not want anything like this to ever happen again. Keith: I'll call Nate. He'll bring the backup, and we'll upload and restore everything up until last night. Sandra: Okay.

# Components of Disaster Recovery

Which of the following is unlikely to be a member of the disaster recovery team? (D2, L2.2.3) 

 A. Executive Management
Incorrect. Executive management should approve the plan and should be provided with a high-level summary of the plan.

 B. Public Relations
Incorrect. Public Relations should be a member of the disaster recovery plan to handle communications to all stakeholders.

 C. Billing Clerk
Correct. A billing clerk is not typically part of the disaster recovery team.

 D. IT Personnel 
Incorrect. IT Personnel are primarily responsible for the disaster recovery team.

