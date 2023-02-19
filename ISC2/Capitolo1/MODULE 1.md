# Module 1: Understand the Security Concepts of Information Assurance

Domain D1.1.1, D1.1.2, D1.1.3, D1.1.4, D1.1.5, D1.1.6

## Module Objective

-   L1.1.1 Recognize foundational security concepts of information assurance .

[Download Transcripts](https://learn.isc2.org/d2l/common/dialogs/quickLink/quickLink.d2l?ou=9238&type=coursefile&fileId=build%2fchapter_01%2ftranscripts%2fChapter%201%20Module%201%20Overview.pdf)
TRANSCRIPT
Manny: A career in cybersecurity is dynamic, and in this module, we'll cover the concepts at the heart of it. 
Tasha: That's right, We'll introduce the security concepts of information assurance and cover topics like the CIA triad, authentication, and privacy. 
Manny: The CIA triad? That sounds like something out of a James Bond movie. 
Tasha: CIA is a basic principle behind everything we do in cybersecurity. Let's find out more.

# Susan's Morning Cup of Joe
Tasha: Now that we've heard a little bit about cybersecurity as a profession, do you know who's a great person to learn more from? Manny: Who? 
Tasha: Susan! She's an SSCP, which means she earned her Systems Security Certified Practitioner certification from (ISC)2 . She's working as a data security analyst, and with the SSCP certification, her career is taking off. Susan stops into JavaSip every morning for a cup of coffee on her way to work. This morning, she observes that Keith is looking sad. 
Susan: Hey, Keith. You having a hard morning? You seem a little down. 
Keith: Yeah, I was up late last night, searching the internet trying to figure out what to do with my life. You're in cybersecurity, right? 
Susan: Mm-hmm. 
Keith: Yeah, I was searching the internet and found out that that's one of the fastest growing careers, but what does that even mean? 
Susan: Well, yes, I am in cybersecurity, and it means that I protect online data from being stolen or altered. Yeah, I assess risks to our network and respond with various safeguards. You think you might be interested in cybersecurity? 
Keith: Oh, no. I'm not that good with computers. Plus, I took a computer programming class in high school and that didn't turn out too well. So don't ask me if I was good at math because I'm not. Besides, I couldn't sit at a desk and code all day. 
Susan: Keith, cybersecurity professionals do not have to be coders, you know? I've seen you on the coffee shop's laptop and on your own devices a lot. You seem pretty knowledgeable to me. 
Keith: Yeah, but cybersecurity seems intimidating. It's like you have to be a tech expert or something, like you. 
Susan: Let me put it this way. You know the fire inspectors who come to JavaSip every year? They check to make sure the building aligns with safety standards and that you have smoke alarms and escape routes. 
Keith: Yeah. I always appreciate a good report. 
Susan: Yeah, well, part of my job is a lot like the fire inspector. I check to make sure the infrastructure aligns with standards, both in the physical building and in the way we handle our data, and I check to make sure that everybody knows what to do in case of an emergency. If a problem does occur, then I'm a little like a paramedic trying to assess and treat any injuries after an accident. Then, I might behave like a detective, tracking down what happened so it doesn't happen again. Sometimes, I even feel like a fortune teller trying to predict the future so that we can be protected against any unknown threats. 
Keith: Yeah. That seems like an interesting image, all right?
Susan: Yeah. Does that sort of thing appeal to you? Because I have heard you say that you want to help people in a meaningful way, and in cybersecurity you can help all kinds of people, companies, and even the world protect personal information and online data. 
Keith: Yeah. I'd like to learn more about it. Thanks, Susan. Susan: Yeah, I'd love to chat more, but I should get to the office now. I don't want any bad actors penetrating our computer network while I'm out enjoying a cup of coffee. Have a good day, Keith. 
Keith: You, too
# The CIA Triad

To define security, it has become common to use Confidentiality, Integrity and Availability, also known as the CIA triad. The purpose of these terms is to describe security using relevant and meaningful words that make security more understandable to management and users and define its purpose. 

_Select each plus sign hotspot to learn more about each topic._

**Confidentiality**  
Confidentiality relates to permitting authorized access to information, while at the same time protecting information from improper disclosure.

**Integrity**  
Integrity is the property of information whereby it is recorded, used and maintained in a way that ensures its completeness, accuracy, internal consistency and usefulness for a stated purpose.

**Availability**  
Availability means that systems and data are accessible at the time users need them.


# CIA Triad Deep Dive
# CIA Triad Deep Dive

_Click on each tab to learn more._ 

![alt text](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/assets/EDU-ELCC-02270a-techart-cia_triad-v04.svg?ou=9541 "alt text")

[Confidentiality](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#) is a difficult balance to achieve when many system users are guests or customers, and it is not known if they are accessing the system from a compromised machine or vulnerable mobile application. So, the security professional’s obligation is to regulate access—protect the data that needs protection, yet permit access to authorized individuals.

[Personally Identifiable Information (PII)](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#) is a term related to the area of confidentiality. It pertains to any data about an individual that could be used to identify them. Other terms related to confidentiality are [protected health information (PHI)](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#) , which is information regarding one’s health status, and [classified or sensitive information](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#), which includes trade secrets, research, business plans and intellectual property.

Another useful definition is [sensitivity](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#), which is a measure of the importance assigned to information by its owner, or the purpose of denoting its need for protection. Sensitive information is information that if improperly disclosed (confidentiality) or modified (integrity) would harm an organization or individual. In many cases, sensitivity is related to the harm to external stakeholders; that is, people or organizations that may not be a part of the organization that processes or uses the information

![alt text](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/assets/EDU-ELCC-02270b-techart-cia_triad-v04.svg?ou=9541 "alt text")

**Integrity** measures the degree to which something is whole and complete, internally consistent and correct. The concept of integrity applies to:

-   information or data
-   systems and processes for business operations
-   organizations
-   people and their actions

[Data integrity](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#) is the assurance that data has not been altered in an unauthorized manner. This requires the protection of the data in systems and during processing to ensure that it is free from improper modification, errors or loss of information and is recorded, used and maintained in a way that ensures its completeness. Data integrity covers data in storage, during processing and while in transit.

Information must be accurate, internally consistent and useful for a stated purpose. The internal consistency of information ensures that information is correct on all related systems so that it is displayed and stored in the same way on all systems. Consistency, as part of data integrity, requires that all instances of the data be identical in form, content and meaning.

[System integrity](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#) refers to the maintenance of a known good configuration and expected operational function as the system processes the information. Ensuring integrity begins with an awareness of [state](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#), which is the current condition of the system. Specifically, this awareness concerns the ability to document and understand the state of data or a system at a certain point, creating a baseline. For example, a [baseline](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#) can refer to the current state of the information—whether it is protected. Then, to preserve that state, the information must always continue to be protected through a transaction.

Going forward from that baseline, the integrity of the data or the system can always be ascertained by comparing the baseline with the current state. If the two match, then the integrity of the data or the system is intact; if the two do not match, then the integrity of the data or the system has been compromised. Integrity is a primary factor in the reliability of information and systems.

The need to safeguard information and system integrity may be dictated by laws and regulations. Often, it is dictated by the needs of the organization to access and use reliable, accurate information.

![alt text](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/assets/EDU-ELCC-02270c-techart-cia_triad-v04.svg?ou=9541 "alt text")

[Availability](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#) can be defined as (1) timely and reliable access to information and the ability to use it, and (2) for authorized users, timely and reliable access to data and information services.

The core concept of availability is that data is accessible to authorized users when and where it is needed and in the form and format required. This does not mean that data or systems are available 100% of the time. Instead, the systems and data meet the requirements of the business for timely and reliable access.

Some systems and data are far more critical than others, so the security professional must ensure that the appropriate levels of availability are provided. This requires consultation with the involved business to ensure that critical systems are identified and available. Availability is often associated with the term [criticality](read://https_learn.isc2.org/?url=https%3A%2F%2Flearn.isc2.org%2Fcontent%2Fenforced%2F9541-CC-SPT-GLOBAL-1ED-1M%2Fbuild%2Fchapter_01%2Fmodule_01%2Fch01-m01-CIA_Triad_Deep_Dive.html%3Fd2lSessionVal%3DINWywuo0tnJv5P4O6sN2kWZ3L%26ou%3D9541%26d2l_body_type%3D3%23#), because it represents the importance an organization gives to data or an information system in performing its operations or achieving its mission.
[Confidentiality](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-CIA_Triad_Deep_Dive.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#) is a difficult balance to achieve when many system users are guests or customers, and it is not known if they are accessing the system from a compromised machine or vulnerable mobile application. So, the security professional’s obligation is to regulate access—protect the data that needs protection, yet permit access to authorized individuals.

[Personally Identifiable Information (PII)](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-CIA_Triad_Deep_Dive.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#) is a term related to the area of confidentiality. It pertains to any data about an individual that could be used to identify them. Other terms related to confidentiality are [protected health information (PHI)](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-CIA_Triad_Deep_Dive.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#) , which is information regarding one’s health status, and [classified or sensitive information](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-CIA_Triad_Deep_Dive.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#), which includes trade secrets, research, business plans and intellectual property.

Another useful definition is [sensitivity](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-CIA_Triad_Deep_Dive.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#), which is a measure of the importance assigned to information by its owner, or the purpose of denoting its need for protection. Sensitive information is information that if improperly disclosed (confidentiality) or modified (integrity) would harm an organization or individual. In many cases, sensitivity is related to the harm to external stakeholders; that is, people or organizations that may not be a part of the organization that processes or uses the information


 # CIA in the Real World
 
 
 Narrator: It’s important to have a comprehensive approach to maintaining the CIA Triad: confidentiality, integrity, and availability. These are the foundations of the cybersecurity domain. 
 
 Confidentiality means that no private information has been disclosed to unauthorized individuals. We need to ensure that personally identifiable information, also known as PII, is protected. If you are part of a security team, your goal is to protect the assets or the information of large corporations or multiple individuals. For example, if you work in banking, health care or insurance companies, you have multiple personal identifiers to protect. 
 
 Integrity ensures that this information is not being corrupted or changed without the information owner’s permission. It confirms that the information being maintained is complete and accurate and consistent with the legitimate use of that information. Interfering with the integrity of information can have serious ramifications. For example, someone without authority changes someone’s medical information, and now a patient may be in jeopardy because someone changed that vital information. Our job is to maintain the security of that information so that no one, unless authorized to do so, changes any part of the information we are protecting. 
 
 Availability is critical because it is essential that authorized users have access to important information in a timely manner. 
 Cyberattacks that disrupt services often target the availability of data. A business cannot function if its employees and customers cannot access their information in a timely manner. 
 A ransomware attack, for example, may lock up a system and block access to vital information and services. That access will not be restored until a payment is made.



# Authentication

When users have stated their identity, it is necessary to validate that they are the rightful owners of that identity. This process of verifying or proving the user’s identification is known as [authentication](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01_m01-Authentication.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#). Simply put, authentication is a process to prove the identity of the requestor.

There are three common methods of authentication:

-   Something you know: Passwords or paraphrases
-   Something you have: [Tokens](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01_m01-Authentication.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#), memory cards, smart cards
-   Something you are: [Biometrics](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01_m01-Authentication.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#) , measurable characteristics

# Methods of Authentication

There are two types of authentication. Using only one of the methods of authentication stated previously is known as [single-factor authentication (SFA)](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-Methods_of_Authentication.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#) . Granting users access only after successfully demonstrating or displaying two or more of these methods is known as [multi-factor authentication (MFA)](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-Methods_of_Authentication.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#) . 

 Common best practice is to implement at least two of the three common techniques for authentication: 

-   Knowledge-based 
-   Token-based 
-   Characteristic-based  

 Knowledge-based authentication uses a passphrase or secret code to differentiate between an authorized and unauthorized user. If you have selected a personal identification number (PIN), created a password or some other secret value that only you know, then you have experienced knowledge-based authentication. The problem with using this type of authentication alone is that it is often vulnerable to a variety of attacks. For example, the help desk might receive a call to reset a user’s password. The challenge is ensuring that the password is reset only for the correct user and not someone else pretending to be that user. For better security, a second or third form of authentication that is based on a token or characteristic would be required prior to resetting the password. The combined use of a user ID and a password consists of two things that are known, and because it does not meet the requirement of using two or more of the authentication methods stated, it is not considered MFA.

# Proving Identity
Narrator: Let us explore authentication a little more. Many of us are already accustomed to different ways of proving who we are, and we do it perhaps without even knowing it. Usually, we are asked to authenticate our identities by using something that we know, such as a password or pass phrase. That is one factor of authentication. Then we use something that only we have, such as a token or card. That gives us two different factors of authentication. When you go to the bank and use your ATM card, you may have a username and password or a specific code, such as a PIN. You HAVE the card, and you KNOW the PIN. So that is one form of multifactor authentication. Someone with just the card cannot access the money. Then, increasingly, we also provide something that we are, with biometrics. This can be a fingerprint or another type of measurable characteristic, such as facial recognition or an iris scan. We see these elements of the authentication process on a daily basis. This adds another layer of multi-factor authentication.

# Non-repudiation

[Non-repudiation](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-Non-repudiation.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#) is a legal term and is defined as the protection against an individual falsely denying having performed a particular action. It provides the capability to determine whether a given individual took a particular action, such as created information, approved information or sent or received a message.

In today’s world of e-commerce and electronic transactions, there are opportunities for the impersonation of others or denial of an action, such as making a purchase online and later denying it. It is important that all participants trust online transactions. Non-repudiation methodologies ensure that people are held responsible for transactions they conducted.

# Privacy

[Privacy](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-Privacy.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#) is the right of an individual to control the distribution of information about themselves. While security and privacy both focus on the protection of personal and sensitive data, there is a difference between them. With the increasing rate at which data is collected and digitally stored across all industries, the push for privacy legislation and compliance with existing policies steadily grows. In today’s global economy, privacy legislation and regulations on privacy and data protection can impact corporations and industries regardless of physical location. Global privacy is an especially crucial issue when considering requirements regarding the collection and security of personal information. There are several laws that define privacy and data protection, which periodically change. Ensuring that protective security measures are in place is not enough to meet privacy regulations or to protect a company from incurring penalties or fines from mishandling, misuse, or improper protection of personal or private information. An example of a law with multinational implications is the European Union’s [General Data Protection Regulation (GDPR)](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/module_01/ch01-m01-Privacy.html?d2lSessionVal=INWywuo0tnJv5P4O6sN2kWZ3L&ou=9541&d2l_body_type=3#) which applies to all organizations, foreign or domestic, doing business in the EU or any persons in the EU. Companies operating or doing business within the United States may also fall under several state legislations that regulate the collection and use of consumer data and privacy. Likewise, member nations of the EU enact laws to put GDPR into practice and sometimes add more stringent requirements. These laws, including national- and state-level laws, dictate that any entity anywhere in the world handling the private data of people in a particular legal jurisdiction must abide by its privacy requirements. As a member of an organization's data protection team, you will not be required to interpret these laws, but you will need an understanding of how they apply to your organization.


# Privacy in the Working Environment

Narrator: Privacy is a major component of information security. Once we know how private the information is, we know what appropriate controls can be implemented. A number of standards, policies and procedures govern privacy in the working environment, and these vary by geographic region. In the United States, HIPAA, the Health Insurance Portability and Accountability Act, controls how the privacy of medical information must be maintained. In the European Union (EU), the General Data Protection Regulation gives anyone within the borders of the EU control over what personal information companies can compile and retain about them. As a security professional, it’s important to be aware of privacy laws and regulations in all jurisdictions where your company conducts business. When doing business in other countries, we must be aware of their privacy standards and regulations and act accordingly

