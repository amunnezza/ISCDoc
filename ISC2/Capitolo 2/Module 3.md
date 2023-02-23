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

Check Answer


## luciano ciotola (username: luciociotola@gmail.com)

## Attempt 1

Written: Feb 23, 2023 7:07 AM - Feb 23, 2023 7:13 AM

## Submission View

Your quiz has been submitted successfully.

**Question 1**

1 / 1 point

You are working in your organization's security office. You receive a call from a user who has tried to log in to the network several times with the correct credentials, with no success. This is an example of a(n)_______. (D2, L2.1.1)

Question options:

A) 

Emergency

B) 

Event

C) 

Policy

D) 

Disaster

View question 1 feedback

**Question 2**

1 / 1 point

You are working in your organization's security office. You receive a call from a user who has tried to log in to the network several times with the correct credentials, with no success. After a brief investigation, you determine that the user's account has been compromised. This is an example of a(n)_______. (D2, L2.1.1)

Question options:

A) 

Risk management

B) 

Incident detection

C) 

Malware

D) 

Disaster

View question 2 feedback

**Question 3**

0 / 1 point

An external entity has tried to gain access to your organization's IT environment without proper authorization. This is an example of a(n) _________. (D2, L2.1.1)

Question options:

A) 

Exploit

B) 

Intrusion

C) 

Event

D) 

Malware

Hide question 3 feedback

Incorrect. While this is, in the most general sense, an event (because it is something in the IT environment that can be measured), the term "intrusion" is a much more specific, accurate description of the situation, so B is a better answer.

**Question 4**

1 / 1 point

When responding to a security incident, your team determines that the vulnerability that was exploited was not widely known to the security community, and that there are no currently known definitions/listings in common vulnerability databases or collections. This vulnerability and exploit might be called ______. (D2, L 2.1.1)

Question options:

A) 

Malware

B) 

Critical

C) 

Fractal

D) 

Zero-day

View question 4 feedback

**Question 5**

1 / 1 point

True or False? The IT department is responsible for creating the organization's business continuity plan. (D2, L2.2.1) 

Question options:

True

False

View question 5 feedback

**Question 6**

1 / 1 point

The Business Continuity effort for an organization is a way to ensure critical ______ functions are maintained during a disaster, emergency, or interruption to the production environment. (D2, L 2.2.1) 

Question options:

A) 

Business

B) 

Technical

C) 

IT

D) 

Financial

View question 6 feedback

**Question 7**

1 / 1 point

Which of the following is very likely to be used in a disaster recovery (DR) effort? (D2, L 2.3.1)

Question options:

A) 

Guard dogs

B) 

Data backups

C) 

Contract personnel

D) 

Anti-malware solutions

View question 7 feedback

**Question 8**

1 / 1 point

Which of the following is often associated with DR planning? (D2, L 2.3.1)

Question options:

A) 

Checklists

B) 

Firewalls

C) 

Motion detectors

D) 

Non-repudiation

View question 8 feedback

**Question 9**

0 / 1 point

Which of these activities is often associated with DR efforts? (D2, L2.3.1)

Question options:

A) 

Employees returning to the primary production location

B) 

Running anti-malware solutions

C) 

Scanning the IT environment for vulnerabilities

D) 

Zero-day exploits

Hide question 9 feedback

Incorrect. Anti-malware is a useful security tool, but it is not typically associated with DR efforts. 

**Question 10**

1 / 1 point

Which of these components is very likely to be instrumental to any disaster recovery (DR) effort? (D2, L2.3.1)

Question options:

A) 

Routers

B) 

Laptops

C) 

Firewalls

D) 

Backups

Hide question 10 feedback

Correct. Backups are often crucial in DR efforts, so that the normal production environment can be restored. 

![Happy face](https://learn.isc2.org/d2l/img/0/Quizzes.Main.actFeedbackHappy.svg?v=20.23.2.16271 "Happy face")

**Congratulations, you passed the quiz!**

You've achieved an overall grade of 70% or higher and completed this activity.

---

**Attempt Score:** 

80 %

**Overall Grade (highest attempt):** 

80 %