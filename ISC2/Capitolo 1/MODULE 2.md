# Module 2: Understand the Risk Management Process

Domain D1.2.1, D1.2.2

## Module Objectives

-   L1.2.1 Define risk management terminology and summarize the process.
-   L1.2.2 Relate risk management to personal or professional practices.

Risks and security-related issues represent an ongoing concern of businesses as well as the field of cybersecurity, but far too often organizations fail to proactively manage risk. Assessing and analyzing risk should be a continuous and comprehensive exercise in any organization. As a member of an organization’s security team, you will work through risk assessment, analysis, mitigation, remediation and communication.

There are many frameworks and models used to facilitate the **risk management** ( _Def. The process of identifying, evaluating and controlling threats, including all the phases of risk context (or frame), risk assessment, risk treatment and risk monitoring._) process, and each organization makes its own determination of what constitutes risk and the level of risk it is willing to accept. However, there are commonalities among the terms, concepts and skills needed to measure and manage risk. This module gets you started by presenting foundational terminology and introducing you to the risk management process.

First, a definition of  **risk**( Def; _A possible event which can have a negative impact upon the organization."_)  is  a measure of the extent to which an entity is threatened by a potential circumstance or event. It is often expressed as a combination of:

1.  the adverse impacts that would arise if the circumstance or event occurs,  and 
2.  the likelihood of occurrence. 

**Information security risk** (Def: _The potential adverse impacts to an organization’s operations (including its mission, functions and image and reputation), assets, individuals, other organizations, and even the nation, which results from the possibility of unauthorized access, use, disclosure, disruption, modification or destruction of information and/or information systems._ ) reflects the potential adverse impacts that result from the possibility of unauthorized access, use, disclosure, disruption, modification or destruction of information and/or information systems. This definition represents that risk is associated with threats, impact and likelihood, and it also indicates that IT risk is a subset of business risk.
# Introduction to Risk Management

## introToRiskManage.mkv
Narrator: Information assurance and cybersecurity are greatly involved with the risk management process. The level of cybersecurity required depends on the level of risk the entity is willing to accept; that is, the potential consequences of what's going on in our environment. Once we evaluate this risk, then we will implement security controls to mitigate the risk to the level that we find acceptable. Risks can be from cyberattacks, such as malware, social engineering, or denial-of-service attacks, or from other situations that affect our environment, such as fire, violent crime, or natural disasters. With well-designed risk management technologies, we can recognize vulnerabilities and threats, and calculate the likelihood and the potential impact of each threat

# Importance of Risk Management

## importanceRiskManage.mkv

transcript
Narrator: What do we mean when we say threats and vulnerabilities? A vulnerability is a gap or weakness in an organization’s protection of its valuable assets, including information. A threat is something or someone that aims to exploit a vulnerability to gain unauthorized access. 
By exploiting a vulnerability, the threat can harm an asset. For example, a natural disaster, such as a major storm, poses a threat to the utility power supply, which is vulnerable to flooding. The IT environment where production takes place is an asset. If the utility power supply is cut off by a storm, the asset might be made unavailable, because the IT components won’t work without power. Our job is to evaluate how likely it is that an event will take place and take appropriate actions to mitigate the risk.

# Risk Management Terminology

Security professionals use their knowledge and skills to examine operational risk management, determine how to use risk data effectively, work cross-functionally and report actionable information and findings to the stakeholders concerned. Terms such as threats, vulnerabilities and assets are familiar to most cybersecurity professionals.

-   An **asset** (_Def. Anything of value that is owned by an organization. Assets include both tangible items such as information systems and physical property and intangible assets such as intellectual property_) is something in need of protection.
-   A **vulnerability**(_Def. Weakness in a information systems, system security procedures, internal controls or implementation that could be exploited by a threat source. NIST SP 800-30 REV. 1_) is a gap or weakness in those protection efforts.
-   A **threat** (_DEF. any circumstance or event with the potential ro adversely impact organizational operarions (including mission, functions, image or reputation) organizational assets, individuals, other organizations or the nation through an information system via unauthorized access, destruction, disclosure, modification of information and/or denial of service. NIST SP 800-30 REV. 1_) is something or someone that aims to exploit a vulnerability to thwart protection efforts.

Risk is the intersection of these terms. Let's look at them more closely.

# Threats

A threat is a person or thing that takes action to exploit (or make use of) a target organization’s system vulnerabilities, as part of achieving or furthering its goal or objectives. To better understand threats, consider the following scenario:

##  Threats.mkv video

Narrator: Tourists are popular targets for pickpockets. The existence of pickpockets in a crowded tourist spot is a threat to the people gathered there. That threat applies to everyone in the vicinity, even other pickpockets. If you are in the vicinity and the pickpocket has identified you as a target, you are facing a threat actor whether you know it or not. The approach and technique taken by the pickpocket is their threat vector

In the context of cybersecurity, typical **threat actors**(_def: An individual or a group that attempts to exploit vulnerabilities to cause or force a threat to occur._) include the following:
-   Insiders (either deliberately, by simple human error, or by gross incompetence).
-   Outside individuals or informal groups (either planned or opportunistic, discovering vulnerability).
-   Formal entities that are nonpolitical (such as business competitors and cybercriminals).
-   Formal entities that are political (such as terrorists, nation-states, and hacktivists).
-   Intelligence or information gatherers (could be any of the above).
-   Technology (such as free-running **bots**( _def Maliciuous code that acts like a remotely controlled ROBOT for an attacker, with other Trojan and worm capabilities_) and **artificial intelligence**( _def. the ability of a computers and robots to simulate human intelligence and behavior_ ) , which could be part of any of the above).

_***Threat Vector:** The means by which a threat actor carries out their objectives._

# Vulnerabilities

A 
>[!vulnerability]- 
> Weakness in a information systems, system security procedures, internal controls or implementation that could be exploited by a threat source. NIST SP 800-30 REV. 1

is an inherent weakness or flaw in a system or component, which, if triggered or acted upon, could cause a risk event to occur. Consider the pickpocket scenario from below.

An organization’s security team strives to decrease its vulnerability. To do so, they view their organization with the eyes of the threat actor, asking themselves, “Why would we be an attractive target?” The answers might provide steps to take that will discourage threat actors, cause them to look elsewhere or simply make it more difficult to launch an attack successfully. For example, to protect yourself from the pickpocket, you could carry your wallet in an inside pocket instead of the back pant pocket or behave alertly instead of ignoring your surroundings. Managing vulnerabilities starts with one simple step: Learn what they are.

## video Vulnerabilities.mkv

Narrator: Let's say the pick pocket chooses you as a target because they see that it will be easier or more profitable to steal from you. Maybe you are distracted, have jewelry that is easy to snatch, or appear weak and less likely to put up a struggle. In other words, you appear more vulnerable than the other tourists and the pick pocket feels that they can exploit that vulnerability or weakness.

# Likelihood

When determining an organization’s vulnerabilities, the security team will consider the **probability** (DEF. The chances, or likelihood that a given threat is capable of exploiting a given vulnerability or a set of vulnerabilities. NIST SP 800-30 REV.1), or **likelihood**(DEF.  The probability that a potential vulnerability may be exercised within the construct of the associated threat environment) , of a potential vulnerability being exploited within the construct of the organization’s threat environment. **Likelihood of occurrence** (DEF _A weighted factor base on a subjective analysis of the probability that a givern threat is capable of expliting a given vulnerability or set vulnerabilities_) is a weighted factor based on a subjective analysis of the probability that a given threat or set of threats is capable of exploiting a given vulnerability or set of vulnerabilities.

Finally, the security team will consider the likely results if a threat is realized and an event occurs. **Impact** (DEF: _The magnitude of harm that could be caused by a threat's exercise of a vulnerability_) is the magnitude of harm that can be expected to result from the consequences of unauthorized disclosure of information, unauthorized modification of information, unauthorized destruction of information, or loss of information or information system availability.

 Think about the impact and the chain of reaction that can result when an event occurs by revisiting the pickpocket scenario:

## video Likelihood.mkv

Narrator: How do the pickpocket’s actions affect your ability to continue your journey? If you appear to be a weak target and the pickpocket chooses to take your money by brute force, will you be able to obtain more cash to complete your vacation or even return home? The downstream impact must also be considered. What if you are injured and require medical treatment or even hospitalization? Impact does not often stop with the incident itself.

# Risk Identification

How do you identify risks? Do you walk down the street watching out for traffic and looking for puddles on the ground? Maybe you’ve noticed loose wires at your desk or water on the office floor? If you’re already on the lookout for risks, you’ll fit with other security professionals who know it’s necessary to dig deeper to find possible problems.  

In the world of cyber, identifying risks is not a one-and-done activity. It’s a recurring process of identifying different possible risks, characterizing them and then estimating their potential for disrupting the organization.  

It involves looking at your unique company and analyzing its unique situation. Security professionals know their organization’s strategic, tactical and operational plans.

Takeaways to remember about risk identification: 

-   Identify risk to communicate it clearly. 
-   Employees at all levels of the organization are responsible for identifying risk.
-   Identify risk to protect against it. 

As a security professional, you are likely to assist in risk assessment at a system level, focusing on process, control, monitoring or incident response and recovery activities. If you’re working with a smaller organization, or one that lacks any kind of risk management and mitigation plan and program, you might have the opportunity to help fill that planning void.
# Risk Assessment

**Risk assessment** ( DEF: _The analysis performed as part of risk managment which incorporates threat adn vulnerability analyses and considers mitigations provided by security controls planned or in place_) is defined as the process of identifying, estimating and prioritizing risks to an organization’s operations (including its mission, functions, image and reputation), assets, individuals, other organizations and even the nation. Risk assessment should result in aligning (or associating) each identified risk resulting from the operation of an information system with the goals, objectives, assets or processes that the organization uses, which in turn aligns with or directly supports achieving the organization’s goals and objectives. 

A common risk assessment activity identifies the risk of fire to a building. While there are many ways to mitigate that risk, the primary goal of a risk assessment is to estimate and prioritize. For example, fire alarms are the lowest cost and can alert personnel to evacuate and reduce the risk of personal injury, but they won’t keep a fire from spreading or causing more damage. Sprinkler systems won’t prevent a fire but can minimize the amount of damage done. However, while sprinklers in a data center limit the fire’s spread, it is likely they will destroy all the systems and data on them. A gas-based system may be the best solution to protect the systems, but it might be cost-prohibitive. A risk assessment can prioritize these items for management to determine the method of mitigation that best suits the assets being protected. 

The result of the risk assessment process is often documented as a report or presentation given to management for their use in prioritizing the identified risk(s). This report is provided to management for review and approval. In some cases, management may indicate a need for a more in-depth or detailed risk assessment performed by internal or external resources.
# Risk Treatment 

**Risk treatment** ( _DEF: The determination of the best way to address an identified risk_) relates to making decisions about the best actions to take regarding the identified and prioritized risk. The decisions made are dependent on the attitude of management toward risk and the availability — and cost — of risk mitigation. The options commonly used to respond to risk are:

Select each plus sign hotspot to learn more about each topic.
![[risk Treatment.png]]
Risk avoidance is the decision to attempt to eliminate the risk entirely. This could include ceasing operation for some or all of the activities of the organization that are exposed to a particular risk. Organization leadership may choose risk avoidance when the potential impact of a given risk is too high or if the likelihood of the risk being realized is simply too grea

Risk acceptance is taking no action to reduce the likelihood of a risk occurring. Management may opt for conducting the business function that is associated with the risk without any further action on the part of the organization, either because the impact or likelihood of occurrence is negligible, or because the benefit is more than enough to offset that risk.

Risk mitigation is the most common type of risk management and includes taking actions to prevent or reduce the possibility of a risk event or its impact. Mitigation can involve remediation measures, or controls, such as security controls, establishing policies, procedures, and standards to minimize adverse risk. Risk cannot always be mitigated, but mitigations such as safety measures should always be in place.

Risk transference is the practice of passing the risk to another party, who will accept the financial impact of the harm resulting from a risk being realized in exchange for payment. Typically, this is an insurance policy.

# Risk Management Process

video: RiskManageProcess.mkv

Narrator: As we mentioned before, an asset is something that we need to protect. It can be information, or it can be an actual physical piece of equipment, such as a rack in the server room or a computer or tablet or even a phone. A vulnerability is a weakness in the system. It can be due to lack of knowledge, or possibly outdated software. For example, perhaps we don't have a current operating system, or our awareness training is lacking. A threat is something or someone that could cause harm once they learn that we have a weakness. For example, if we have a back door open, either logically, in our website, or even physically in the back office, someone can exploit that weakness and take advantage of that gap in our defenses to access information. The likelihood or the probability of that happening depends on the overall environment. In an environment that's extremely secure, such as a data center or a bank, the likelihood that someone can come in and rob the bank is very low. Whether they are seeking access through a web browser, or physically into the actual bank, their likelihood of success is not high because security is very strong. In other situations, where we have fewer levels of security, the likelihood that the environment can be compromised is much higher. In our daily accounts, we often only have one username and a password and that is the extent of our defenses. Anyone who obtains that username and password can gain access; therefore, the likelihood that this environment can be compromised is very high. As a first step in the risk management process, organizations need to figure out how much risk they are willing to take. This is called a risk appetite or risk tolerance. For a very trivial example, if you are a big fan of football or a particular TV program, you will have a low tolerance for having a power outage during a big game or your favorite program. You also need to have power when you are trying to access important documents or sites for your business, so your risk appetite depends on how important that asset is. If your data is extremely sensitive, you will naturally be extremely averse to having any risk of a breach. To mitigate the risk, one option is to hire another company with the expertise to help you maintain the security of your environment. This will help reduce the risk. You would also consider implementing some security controls, which we will explore shortly. If we don't have the competence or the means to protect sensitive information, sometimes we need to avoid the risk. This means removing ourselves from a situation that can result in problems and refraining from initiating risky activities until we achieve a certain level of comfort with our security. We can also share or transfer the risk by obtaining cybersecurity insurance, so the insurance company assumes the risk. While it is nearly impossible to remove all risk, once we have done enough to reduce or transfer the risk, and we are comfortable with the situation, then we can accept the level of risk that remains

![[termini.png]]


# Risk Treatment 

When a company chooses to ignore a risk and proceed with a risky activity, which treatment is being applied by default? (D1, L1.2.2)

 A. Mitigation

Incorrect. Mitigation involves taking action to remove or lessen the effects of risks.

 B. Avoidance

Incorrect. Avoidance is halting the risky activity.

 C. Acceptance

Correct. Acceptance is choosing to ignore a risk and proceed with a risky activity.

 D. Transference

Incorrect. Transference is shifting the risk via legal agreement, usually to another party such as a service or insurance provider.
# Risk Management: Susan’s Good News

video : RiskManageSusan.mkv

Manny: The last time we saw Susan, she stepped into JavaSip for a cup of coffee and spoke to Keith about her job as a data security analyst in a security operations center. Tasha: Or, as Susan calls it, the SOC. 
Manny: But what is a SOC, anyway? 
Tasha: It's like headquarters for an information security team. That's where they monitor, detect, and analyze events on the network so they can prevent and resolve issues before they disrupt the business. 
Manny: That sounds cool. Well, I bet with her coffee in hand, Susan is ready for another busy day at the fast-paced environment of the SOC. Tasha: That's right. Let's see how it's going for her. Manny: It's a good day for Susan. Upon arriving at the SOC where she's worked for two years as a senior data security analyst, Susan hears that she's just been promoted to manager. Tasha: That's so exciting! Now, she reports directly to the chief information security officer, known as a CISO. Manny: And she's now responsible for the management, operations, safety, and security of the SOC. Tasha: That must have been some cup of coffee. Let's listen in as she makes a presentation to her boss and colleagues just a few days after the promotion. Susan: Hi, everyone. Thank you all for coming. Okay, so one of my first goals in my new role was assessing the skill set of our current staff and highlighting the current and future needs of the SOC. Using a template provided by our CISO, I carefully considered the company's goals, as well as the milestones of the larger projects and considered staffing needs. During this process, I identified a risk in relation to staffing and conducted an assessment. I plan to make a recommendation on whether the company should mitigate, avoid, transfer, or accept this risk. Tasha: Evaluating risk is a big part of Susan's new job. Let's hear a little more about how she does this. Susan: As we all know, our staff is a dynamic team challenged by the volume and growing sophistication of the cyber threat alerts that they are receiving. Because of the fast pace and the high level of manual triage needed to address these threats, there is a potential for high turnover among the Tier One and the Tier Two incident response teams. And because hiring, onboarding, and training new staff takes time, turnover could mean that there are fewer trained associates available to triage or escalate these threats. The training of new staff is not only time-consuming and costly, but it also represents an increased cyber risk to the company. Now, I have access to some data, including quarterly hiring reports from HR and the number of incidents that are triaged each week, but I decided that I didn't have enough information to do a quantitative risk assessment. However, a qualitative risk assessment may be well-suited for this situation because it allows us to rank or estimate the probability of a particular risk occurring and the loss or impact of that risk using terms such as high, low, moderate, and severe. This will provide me with enough information in my report to allow the leadership team to decide if any further analysis is needed. Tasha: Susan can use a graphical representation to help her evaluate and communicate potential risk. Susan: Now, I'm going to use a risk matrix to determine the likelihood of the operational risk occurring. Having worked in the SOC myself for several years, I have personally witnessed a high turnover rate among the SOC staff. So, I think that there is a moderate to high chance of the risk occurring, meaning this risk belongs in the upper quadrants of the matrix. And I just need to figure out if the risk carries a high or low impact on the organization as a whole. Manny: When Susan determines the quadrant, which will be covered more shortly, she can include in her report a recommendation suggesting risk mitigation, avoidance, transference, or acceptance. Tasha: This recommendation could also help company management to prioritize the risk and enable the organization to balance immediate and longer-term cost and benefits. Manny: Good work, Susan. We know you'll do great in your new position.

# Risk in Our Lives
video RiskLives.mkv

Narrator: On a personal level, one example of a threat and its impact is unauthorized charges on your credit card. It’s a good idea not to store your credit information in your phone or on your web browser, even though that is convenient for online shopping. Most banks won’t charge you for unauthorized purchases, but it may result in your account being frozen when you are trying to use it, or the hassle of replacing a card that has been compromised and updating any subscriptions or bills that were paid directly with that card. If you identify a risk beforehand, you can mitigate it by adding layers of security, such as multifactor authorization. Most bank websites either require or at least encourage you to set up multifactor authentication when you access your account, so you need a username and password and also a code sent to your email or your cellphone. Another example of handling risk is when you book a vacation. For example, you might be considering a Caribbean cruise where the weather can be a factor and your trip could be cancelled. In that case, you purchase travel insurance to transfer the risk, so you don’t lose out on your prepaid expenses and deposits if something happens to prevent the trip. Other types of insurance are also ways to transfer risk. You might purchase additional health care coverage, to cover your expenses if you have an accident. If you are concerned about identity theft, there are companies that offer an insurance policy for managing your identity. These companies are involved in their own form of financial risk management, calculating that your premium payments or subscription payments will exceed the payouts they will have to make in the event of a claim

# Risk Priorities

When risks have been identified, it is time to prioritize and analyze core risks through **qualitative risk analysis** (DEF_ _A method for risk analysis that is based on the assignmento of a descriptor such as low, medium or high. NISIT 8286_) and/or **quantitative risk analysis** (DEF: _A method for risk analysis where numerical values are assigned to both impact and likelihood based on statistical probabilities and monetarized valuation of loss or gain. Source NISTIR 8286_). This is necessary to determine root cause and narrow down apparent risks and core risks. Security professionals work with their teams to conduct both qualitative and quantitative analysis. 

Understanding the organization’s overall mission and the functions that support the mission helps to place risks in context, determine the root causes and prioritize the assessment and analysis of these items. In most cases, management will provide direction for using the findings of the risk assessment to determine a prioritized set of risk-response actions.![chart showing priority increasing as risk moves from low probability and low impact to high probability and high impact](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/assets/EDU-ELCC-70063-techart-risk_management-v01.svg?_&d2lSessionVal=ohNtLgLXUk56ZvW7pBSN3nQPY&ou=9541)

One effective method to prioritize risk is to use a risk matrix, which helps identify priority as the intersection of likelihood of occurrence and impact. It also gives the team a common language to use with management when determining the final priorities. For example, a low likelihood and a low impact might result in a low priority, while an incident with a high likelihood and high impact will result in a high priority. Assignment of priority may relate to business priorities, the cost of mitigating a risk or the potential for loss if an incident occurs.

# Decision Making Based on Risk Priorities

When making decisions based on risk priorities, organizations must evaluate the likelihood and impact of the risk as well as their tolerance for different sorts of risk. A company in Hawaii is more concerned about the risk of volcanic eruptions than a company in Chicago, but the Chicago company will have to plan for blizzards. In those cases, determining risk tolerance is up to the executive management and board of directors. If a company chooses to ignore or accept risk, exposing workers to asbestos, for example, it puts the company in a position of tremendous liability.
# Risk Tolerance

The perception management takes toward risk is often likened to the entity’s appetite for risk. How much risk are they willing to take? Does management welcome risk or want to avoid it? The level of **risk tolerance** (DEF: _The level of risk an entity is willing to assume in order to achieve a potential desired result. Risk threshold, risk appetite and acceptable risk are also terms used synomously with risk tolerance_) varies across organizations, and even internally: Different departments may have different attitudes toward what is acceptable or unacceptable risk.

Understanding the organization and senior management’s attitude toward risk is usually the starting point for getting management to take action regarding risks.

Executive management and/or the Board of Directors determines what is an acceptable level of risk for the organization. Security professionals aim to maintain the levels of risk within management’s limit of risk tolerance.

Often, risk tolerance is dictated by geographic location. For example, companies in Iceland plan for the risks that nearby volcanoes impose on their business. Companies that are outside the projected path of a lava flow will be at a lower risk than those directly in the path’s flow. Similarly, the likelihood of a power outage affecting the data center is a real threat in all areas of the world. In areas where thunderstorms are common, power outages may occur more than once a month, while other areas may only experience one or two power outages annually. Calculating the downtime that is likely to occur with varying lengths of downtime will help to define a company’s risk tolerance. If a company has a low tolerance of the risk of downtime, they are more likely to invest in a generator to power critical systems. A company with an even lower tolerance for downtime will invest in multiple generators with multiple fuel sources to provide a higher level of assurance that the power will not fail.

# Risk Tolerance Drives Decision Making

## RiskDecisionMaking.mkv video

Narrator: Here are a few examples of how risk tolerance can drive decision making for organizations.
• An organization is required to build a bid package to gain a contract. The time and effort of personnel building a bid package will cost the organization $10,000 USD. If the organization wins the contract, the contract pays $2,000,000 USD. The organization decides to accept the risk of losing the cost of the bid package, because the benefit of winning the contract is appealing. The risk of losing the bid (and the cost of building the bid package) is within the organization’s risk threshold. 
• A trauma center has three critical-care units where patients are provided lifesustaining services (breathing and heart activity) through the use of machines. Inactivity of these machines could mean that people will die. The trauma center has zero tolerance for power failure, so creates redundant emergency power supplies, through the use of multiple utility power providers, battery backup, and multiple generators with secure fuel supplies and solid contracts with fuel providers to deliver additional fuel during emergency situations.
• Liza and Krith think they can build a business that is profitable and enjoyable; they decide to quit their jobs and start the business together. They tolerate the risk that their business might fail because the reward they perceive is significant.

# Swimming with Sharks

file: SwimwithShark.mp3

Josh: Welcome to Dancing with Danger. A travel podcast about risk-loving people doing risky things. I'm Joshua Justin and today I'm talking with Sarah McMillan who runs the Swimming with Sharks attraction here in sunny Key West, Florida. Hi Sarah, how you doing today? 
Sarah: It's a beautiful day to be swimming with sharks in Florida, Josh. 
Josh: Some might disagree. Wouldn't you say this is a particularly risky thing to do? Downright dangerous in fact. 
Sarah: Everything is risky, Josh, from driving in a car to giving your credit card number to a telemarketer. Well in our business, people are lowered into the water in steel cages to observe and photograph sharks. Obviously this has some risk attached. The key is that we take risk very seriously and we take steps to make our attraction as safe as possible, both for the participants and for those who have invested in the business. If something were to happen, the bad publicity and the legal liability would take a big bite out of our livelihood. If you pardon the pun. 
Josh: I don't actually, but tell me more about the different ways you address the dangers of your enterprise. Like, the sharks are tame or mechanical or something, right? 
Sarah: No, these are absolutely real wild sharks. That's what's exciting about it. And part of the fun is the danger, or the perception of danger. 
Josh: So it's only a perception? 
Sarah: No, of course not. Well, mostly. 
Josh: I don't think I'm following. Is it dangerous or not? 
Sarah: Okay. Okay. We're going to accept that there are some risks involved here, right? If we weren't willing to accept a little danger we wouldn't be in this business and the customers wouldn't be signing up to participate. Customers who aren't feeling very brave can obviously avoid the risk by not participating. We have a video feed so they can watch other people in the cages. So they get to share the experience. We also avoid risk by not going out in certain weather conditions or when particularly dangerous shark activity has been observed. We keep a very close eye both on the weather and the animal's behavior so we don't take unnecessary chances with our crew or our customers or even our equipment. 
Josh: So you don't go out unless conditions are ideal. What other safeguards do you take? 
Sarah: We mitigate our risk by having very strong cages and testing them often. And we train our crews rigorously to adhere to our safety policies and procedures and to abide by Florida laws and federal safety regulations. 
Josh: What if something happens in spite of all your preparation? People love to sue businesses when accidents happen. 
Sarah: That's why all our participants are required to sign waivers. That serves to mitigate the risk of liability. 
Josh: Do people object to the waivers? 
Sarah: Not really. This sort of risk management approach is very common. Everything you do has fine print, from downloading an app to flying in a plane or staying at a hotel. Even at other attractions, like those run by animated mice and ducks that we will not name, the ticket includes a disclaimer in the fine print that the park is not responsible for theft or accidents on the property. You are responsible for keeping track of your own belongings and your own kids and so on and so on. So people are quite used to accepting such conditions whenever they do just about anything. But we also have an insurance policy to handle any liability claims. This allows us to transfer our risk to another party. The insurance company is taking the gamble that our premiums and those of other businesses, will bring in more income than a potential claim would make them pay out. 
Josh: So you've been in business here for a couple of years now. 
Sarah: That's correct. About two years. 
Josh: And in that time, have you had any liability claims? 
Sarah: Not regarding the sharks. However, we did have a breach regarding our credit card information. That was a headache. Now we outsource our customer management system to a cloud based third party. So they assume the risk for cybersecurity. We discover that human sharks are a much bigger risk than marine sharks. The beach is safer than the breach, I guess you'd say. 
Josh: I don't think I would, but thank you Sarah for taking the time to talk to our listeners today. I know we've learned a lot about shark related safety issues. 
Sarah: You're welcome, Joshua. Thank you again for having me and let me know when you are ready to swim with the sharks. 
Josh: That's all for today's Dancing with Danger episode. Tune into next week when we go bungee jumping with bears.


