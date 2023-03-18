# Module 3: Understand Network Security Infrastructure

Domain D4.3.1, D4.3.2

## Module Objective

-   L4.3.1 Identify common data center terminology.
-   L4.3.2 Recognize common cloud service terminology.
-   L4.3.3 Identify secure network design terminology.
VIDEO
UndestandNetworkInfrastructure.mkv

Manny: In this section, we are going to be exploring the concepts and terminology around data centers and the cloud. Sounds exciting! 
Tasha: It can be, 
Manny. This is where a lot of the future applications of cybersecurity will come from. As threats evolve, so does the technology to improve data protection, wherever that data is stored and however it's transmitted.

# On-Premises Data Centers

When it comes to data centers, there are two primary options: organizations can outsource the data center or own the data center. If the data center is owned, it will likely be built on premises. A place, like a building for the data center is needed, along with power, HVAC, fire suppression and redundancy.

_Select each plus sign hotspot to learn more about each topic._![[
![[2023-03-02 11_29_18-On-Premises Data Centers.png]]

## A- Data Center/Closets

The facility wiring infrastructure is integral to overall information system security and reliability. Protecting access to the physical layer of the network is important in minimizing intentional or unintentional damage. Proper protection of the physical site must address these sorts of security challenges. Data centers and wiring closets may include the following:

-   Phone, network, special connections
-   ISP or telecommunications provider equipment
-   Servers
-   Wiring and/or switch components

## B- Heating, Ventilation and Air Conditioning (HVAC) / Environmental



High-density equipment and equipment within enclosed spaces requires adequate cooling and airflow. Well-established standards for the operation of computer equipment exist, and equipment is tested against these standards. For example, the recommended range for optimized maximum uptime and hardware life is from 64° to 81°F (18° to 27°C), and it is recommended that a rack have three temperature sensors, positioned at the top, middle and bottom of the rack, to measure the actual operating temperature of the environment. Proper management of data center temperatures, including cooling, is essential.

Cooling is not the only issue with airflow: Contaminants like dust and noxious fumes require appropriate controls to minimize their impact on equipment. Monitoring for water or gas leaks, sewer overflow or HVAC failure should be integrated into the building control environment, with appropriate alarms to signal to organizational staff. Contingency planning to respond to the warnings should prioritize the systems in the building, so the impact of a major system failure on people, operations or other infrastructure can be minimized.

## C- Power

Data centers and information systems in general consume a tremendous amount of electrical power, which needs to be delivered both constantly and consistently. Wide fluctuations in the quality of power affect system lifespan, while disruptions in supply completely stop system operations.

Power at the site is always an integral part of data center operations. Regardless of fuel source, backup generators must be sized to provide for the critical load (the computing resources) and the supporting infrastructure. Similarly, battery backups must be properly sized to carry the critical load until generators start and stabilize. As with data backups, testing is necessary to ensure the failover to alternate power works properly.

## D- Fire Suppression

For server rooms, appropriate fire detection/suppression must be considered based on the size of the room, typical human occupation, egress routes and risk of damage to equipment. For example, water used for fire suppression would cause more harm to servers and other electronic components. Gas-based fire suppression systems are more friendly to the electronics, but can be toxic to humans.
****
# Deeper Dive of On-Premises Data Centers

video DeepDiveDataCenter.mkv

Narrator: Now that we have looked at some of the primary components that must be considered when building an on-premises data center, we should take a deeper dive into some of the components. First, we consider the air conditioning requirements of a data center. Servers and other equipment generate a lot of heat which must be handled appropriately. This is not just to make it comfortable when humans are present, but to ensure the equipment is kept within its operating parameters. When equipment gets too hot, it can lead to quicker failure or a voided warranty. Most equipment is programmed to automatically shut down when a certain temperature threshold is met. This helps to protect the equipment, but a system that is shut down is not available to the users. An abnormal system shutdown can also lead to the loss or corruption of data. Another consideration for the on-premises data center is the fire suppression systems. In the United States, most commercial buildings are required to have sprinkler systems that are activated in a fire. These sprinklers minimize the amount of damage caused to the building and keep the fire from spreading to adjacent areas, but they can be detrimental to electronic equipment, as water and electricity don’t mix. While most water-based fire suppression systems don’t work like they do in the movies, where a fire in one part of the building turns on the sprinklers for the entire building, another hazard is having water overhead in a data center. Eventually, water pipes will fail and may leak on equipment. This risk can be reduced somewhat by using a dry-pipe system that keeps the water out of the pipes over the data center. These systems have a valve outside the data center that is only opened when a sensor indicates a fire is present. Since water is not held in the pipes above the data center, the risk of leaks is reduced.
****

# Redundancy

The concept of redundancy is to design systems with duplicate components so that if a failure were to occur, there would be a backup. This can apply to the data center as well. Risk assessments pertaining to the data center should identify when multiple separate utility service entrances are necessary for redundant communication channels and/or mechanisms.  

If the organization requires full redundancy, devices should have two power supplies connected to diverse power sources. Those power sources would be backed up by batteries and generators. In a high-availability environment, even generators would be redundant and fed by different fuel types.

![[Redundancy.png]]

# Example of Redundancy (Application of)

video ExampleRedund.mkv

Narrator: In addition to keeping redundant backups of information, you also have a redundant source of power, to provide backup power so you have an uninterrupted power supply, or UPS. Transfer switches or transformers may also be involved. And in case the power is interrupted by weather or blackouts, a backup generator is essential. Often there will be two generators connected by two different transfer switches. These generators might be powered by diesel or gasoline or another fuel such as propane, or even by solar panels. A hospital or essential government agency might contract with more than one power company and be on two different grids in case one goes out. This is what we mean by redundancy.
****
# Memorandum of Understanding (MOU)/Memorandum of Agreement (MOA) 

Some organizations seeking to minimize downtime and enhance BC (Business Continuity) and DR (Disaster Recovery) capabilities will create agreements with other, similar organizations. They agree that if one of the parties experiences an emergency and cannot operate within their own facility, the other party will share its resources and let them operate within theirs in order to maintain critical functions. These agreements often even include competitors, because their facilities and resources meet the needs of their particular industry. 

For example, Hospital A and Hospital B are competitors in the same city. The hospitals create an agreement with each other: if something bad happens to Hospital A (a fire, flood, bomb threat, loss of power, etc.), that hospital can temporarily send personnel and systems to work inside Hospital B in order to stay in business during the interruption (and Hospital B can relocate to Hospital A, if Hospital B has a similar problem). The hospitals have decided that they are not going to compete based on safety and security—they are going to compete on service, price and customer loyalty. This way, they protect themselves and the healthcare industry as a whole.  

These agreements are called joint operating agreements (JOA) or memoranda of understanding (MOU) or memoranda of agreement (MOA). Sometimes these agreements are mandated by regulatory requirements, or they might just be part of the administrative safeguards instituted by an entity within the guidelines of its industry. 

The difference between an MOA or MOU  and an SLA is that a Memorandum of Understanding is more directly related to what can be done with a system or the information. 

The service level agreement goes down to the granular level. For example, if I'm outsourcing the IT services, then I will need to have two full-time technicians readily available, at least from Monday through Friday from eight to five. With cloud computing, I need to have access to the information in my backup systems within 10 minutes. An SLA specifies the more intricate aspects of the services.  

We must be very cautious when outsourcing with cloud-based services, because we have to make sure that we understand exactly what we are agreeing to. If the SLA promises 100 percent accessibility to information, is the access directly to you at the moment, or is it access to their website or through their portal when they open on Monday? That's where you'll rely on your legal team, who can supervise and review the conditions carefully before you sign the dotted line at the bottom.

# On-Premises

Which of the following is typically associated with an on-premises data center? (D4, L4.3.1) 

A. Fire suppression
Fire suppression is associated with an on-premises data center, but this answer is incorrect. What else might be associated with an on-premises data center?

B. HVAC
HVAC is associated with an on-premises data center, but this answer is incorrect. What else might be associated with an on-premises data center?

C. Power
Power is associated with an on-premises data center, but this answer is incorrect. What else might be associated with an on-premises data center?

D. All of the above
Correct. Fire suppression, HVAC and power are all associated with an on-premises data center.

# Which of the Following is Not a Source of Redundant Power

Which of the following is not a source of redundant power (D4, L4.3.1):  

 A. HVAC
 B. Generator
 C. Utility
 D. UPS

Correct answer: A. HVAC
HVAC is not a source of redundant power, but it is something that needs to be protected by a redundant power supply, which is what the other three options will provide. What happens if the HVAC system breaks and equipment gets too hot? If the temperature in the data center gets too hot, then there is a risk that the server will shut down or fail sooner than expected, which presents a risk that data will be lost. So that is another system that requires redundancy in order to reduce the risk of data loss. But it is not itself a source of redundant power.


# Cloud

>[!Cloud computing]+ 
>A model for enabling ubiquitous, convenient, on demand network access to a share pool of configurable computing resources (e.g. networks, servers, storage, applications, and services) that can be rapidly provisioned and released with mminial management effort or service providerr interaction NIST 800-145
>

is usually associated with an internet-based set of computing resources, and typically sold as a service, provided by a cloud service provider (CSP). 

Cloud computing is very similar to the electrical or power grid. It is provisioned in a geographic location and is sourced using an electrical means that is not necessarily obvious to the consumer. But when you want electricity, it’s available to you via a common standard interface and you pay only for what you use. In these ways, cloud computing is very similar. It is a very scalable, elastic and easy-to-use “utility” for the provisioning and deployment of Information Technology (IT) services.  

There are various definitions of what cloud computing means according to the leading standards, including NIST. This NIST definition is commonly used around the globe, cited by professionals and others alike to clarify what the term “cloud” means:  

_“a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources (such as networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction.” NIST SP 800-145_ 


This image depicts cloud computing characteristics, service and deployment models, all of which will be covered in this section and by your instructor.![[Cloud.png]]


# Cloud Redundancy VIDEO

CLOUDREDUND.MKV

Narrator: Many organizations have moved from hard-wired server rooms to operations that are run by cloud-based facilities, because it provides both security and flexibility. Cloud service providers have different availability zones, so that if one goes down, activities can shift to another. You don’t have to maintain a whole data center with all the redundancy that entails – the cloud service provider does that for you. There are several ways to contract with a cloud service provider. You can set up the billing so that it depends on the data used, just like your mobile phone. And you have resource pooling, meaning you can share in the resources of other colleagues or similar types of industries to provide data for artificial intelligence or analytics.

# Cloud Characteristics

Cloud-based assets include any resources that an organization accesses using cloud computing. Cloud computing refers to on-demand access to computing resources available from almost anywhere, and cloud computing resources are highly available and easily scalable. Organizations typically lease cloud-based resources from outside the organization. Cloud computing has many benefits for organizations, which include but are not limited to: 

-   Usage is metered and priced according to units (or instances) consumed. This can also be billed back to specific departments or functions.
-   Reduced cost of ownership. There is no need to buy any assets for everyday use, no loss of asset value over time and a reduction of other related costs of maintenance and support.
-   Reduced energy and cooling costs, along with “green IT” environment effect with optimum use of IT resources and systems.
-   Allows an enterprise to scale up new software or data-based services/solutions through cloud systems quickly and without having to install massive hardware locally.


# Service Models

Some cloud-based services only provide data storage and access. When storing data in the cloud, organizations must ensure that security controls are in place to prevent unauthorized access to the data. 

There are varying levels of responsibility for assets depending on the service model. This includes maintaining the assets, ensuring they remain functional, and keeping the systems and applications up to date with current patches. In some cases, the cloud service provider is responsible for these steps. In other cases, the consumer is responsible for these steps. 

Types of cloud computing service models include
>[!Software as a Service SaaS]+
> The cloud customer uses the cloud provider's applications running within a cloud infrastructure. The applications are accessible from various client devices through either a thin client interface such as a browser or a program interface. The consumer does not manage or control the underlying clouf infrastructure including network, servvers, operating system, storage or even individual application capabilities, with the possible ixception of limited user-specific application configuration settings. Derived from NIST 800-145


>[!Platform as a Service (PAAS)]+
>The web authoring or application development middleware environment that allows applications to be built in the cloud before they are deployed as SaaS assets.

and 
>[!Infrastructure as a Service (IaaS)]+ 
>The provider of the core computing, storage and network hardware and software that is the foundation upon which organizations can build and than deploy applications. IaaS is popular in the data center where software and serers are purchased as a fully outsourced service and usually billed on usage and how much of the resource is used.

![[Service Models.png]]

##### Software as a Service (SaaS)
Software as a Service (SaaS): A cloud provides access to software applications such as email or office productivity tools. SaaS is a distributed model where software applications are hosted by a vendor or cloud service provider and made available to customers over network resources. SaaS is a widely used and adopted form of cloud computing, with users most often needing an internet connection and access credentials to have full use of the cloud service, application and data. SaaS has many benefits for organizations, which include but are not limited to: Ease of use and limited/minimal administration. Automatic updates and patch management. The user will always be running the latest version and most up-to-date deployment of the software release, as well as any relevant security updates, with no manual patching required. Standardization and compatibility. All users will have the same version of the software release.

##### Platform as a Service (PaaS)
Platform as a Service (PaaS): A cloud provides an environment for customers to use to build and operate their own software. PaaS is a way for customers to rent hardware, operating systems, storage and network capacity over the internet from a cloud service provider. The service delivery model allows customers to rent virtualized servers and associated services for running existing applications or developing and testing new ones. The consumer does not manage or control the underlying cloud infrastructure, including network, servers, operating systems or storage, but has control over the deployed applications and possibly application-hosting environment configurations. A PaaS cloud provides a toolkit for conveniently developing, deploying and administering application software that is structured to support large numbers of consumers, process very large quantities of data and potentially be accessed from any point on the internet. PaaS clouds will typically provide a set of software building blocks and a set of development tools such as programming languages and supporting run-time environments that facilitate the construction of high-quality, scalable applications. Additionally, PaaS clouds will typically provide tools that assist with the deployment of new applications. In some cases, deploying a new software application in a PaaS cloud is not much more difficult than uploading a file to a web server. PaaS clouds will also generally provide and maintain the computing resources (e.g., processing, storage and networking) that consumer applications need to operate. PaaS clouds provide many benefits for developers, including that the operating system can be changed and upgraded frequently, along with associated features and system services.

##### Infrastructure as a Service (IaaS)
Infrastructure as a Service (IaaS): A cloud provides network access to traditional computing resources such as processing power and storage. IaaS models provide basic computing resources to consumers. This includes servers, storage, and in some cases, networking resources. Consumers install operating systems and applications and perform all required maintenance on the operating systems and applications. Although the consumer has use of the related equipment, the cloud service provider retains ownership and is ultimately responsible for hosting, running and maintenance of the hardware. IaaS is also referred to as hardware as a service by some customers and providers. IaaS has a number of benefits for organizations, which include but are not limited to: Ability to scale up and down infrastructure services based on actual usage. This is particularly useful and beneficial where there are significant spikes and dips within the usage curve for infrastructure. Retain system control at the operating system level.



# Deployment Models

There are four cloud deployment models. The cloud deployment model also affects the breakdown of responsibilities of the cloud-based assets. The four cloud models available are
>[!public]+
>The cloud infrastructure is provisioined for open use by the general public. It may be owned managed and operated by a business, academic or government organization, or some combination of them. It exists on the premises of the cloud provider. NIST SP 800-145 

>[!private]+
>The phrase used to describe a cloud computing platformm that is implemented within the corporate firewall , under the control of the IT department. A private cloud is designed to offer the same features and benefits of cloud systems, but removes a number of objections to the cloud computing model, including control over enterprise and customer data, worries about security, and issues connected to regulatory compliance.  

>[!hybrid]+
>A combination of public cloud storage and private cloud storage where some critical data resides in enterprise's private cloud while other data is stored and accessible from a public cloud storage provider. 

and 

>[!community]+
>A system in which the cloud infrastrructure is provisioned for exclusive use by a specific community of consumers from organizations that have shared concerns (e.g. mission, security requirements, policy and compliance considerations). It may be owned, managed and operate by one or more organizations in the community, a third party or some vcombination of them, and it may exists on or off premises NIST 800-145








![[Deployment Models.png]]
##### Public
Public clouds are what we commonly refer to as the cloud for the public user. It is very easy to get access to a public cloud. There is no real mechanism, other than applying for and paying for the cloud service. It is open to the public and is, therefore, a shared resource that many people will be able to use as part of a resource pool. A public cloud deployment model includes assets available for any consumers to rent or lease and is hosted by an external cloud service provider (CSP). Service level agreements can be effective at ensuring the CSP provides the cloud-based services at a level acceptable to the organization.

##### Private
Private clouds begin with the same technical concept as public clouds, except that instead of being shared with the public, they are generally developed and deployed for a private organization that builds its own cloud. Organizations can create and host private clouds using their own resources. Therefore, this deployment model includes cloud-based assets for a single organization. As such, the organization is responsible for all maintenance. However, an organization can also rent resources from a third party and split maintenance requirements based on the service model (SaaS, PaaS or IaaS). Private clouds provide organizations and their departments private access to the computing, storage, networking and software assets that are available in the private cloud.

##### Hybrid
A hybrid cloud deployment model is created by combining two forms of cloud computing deployment models, typically a public and private cloud. Hybrid cloud computing is gaining popularity with organizations by providing them with the ability to retain control of their IT environments, conveniently allowing them to use public cloud service to fulfill non-mission-critical workloads, and taking advantage of flexibility, scalability and cost savings. Important drivers or benefits of hybrid cloud deployments include: Retaining ownership and oversight of critical tasks and processes related to technology, Reusing previous investments in technology within the organization, Control over most critical business components and systems, and Cost-effective means to fulfilling noncritical business functions (utilizing public cloud components).

##### Community
Community clouds can be either public or private. What makes them unique is that they are generally developed for a particular community. An example could be a public community cloud focused primarily on organic food, or maybe a community cloud focused specifically on financial services. The idea behind the community cloud is that people of like minds or similar interests can get together, share IT capabilities and services, and use them in a way that is beneficial for the particular interests that they share.
****
# Managed Service Provider (MSP)

A managed service provider (MSP) is a company that manages information technology assets for another company. Small- and medium-sized businesses commonly outsource part or all of their information technology functions to an MSP to manage day-to-day operations or to provide expertise in areas the company does not have. Organizations may also use an MSP to provide network and security monitoring and patching services. Today, many MSPs offer cloud-based services augmenting SaaS solutions with active incident investigation and response activities. One such example is a managed detection and response (MDR) service, where a vendor monitors firewall and other security tools to provide expertise in triaging events. 

Some other common MSP implementations are: 

-   Augment in-house staff for projects
-   Utilize expertise for implementation of a product or service
-   Provide payroll services
-   Provide Help Desk service management
-   Monitor and respond to security incidents
-   Manage all in-house IT infrastructure
# Service-Level Agreement (SLA)

The cloud computing service-level agreement (cloud SLA) is an agreement between a cloud service provider and a cloud service customer based on a taxonomy of cloud computing– specific terms to set the quality of the cloud services delivered. It characterizes quality of the cloud services delivered in terms of a set of measurable properties specific to cloud computing (business and technical) and a given set of cloud computing roles (cloud service customer, cloud service provider, and related sub-roles).

Think of a rule book and legal contract—that combination is what you have in a service-level agreement (SLA). Let us not underestimate or downplay the importance of this document/ agreement. In it, the minimum level of service, availability, security, controls, processes, communications, support and many other crucial business elements are stated and agreed to by both parties.  

The purpose of an SLA is to document specific parameters, minimum service levels and remedies for any failure to meet the specified requirements. It should also affirm data ownership and specify data return and destruction details. Other important SLA points to consider include the following:

-   Cloud system infrastructure details and security standards
-   Customer right to audit legal and regulatory compliance by the CSP         
-   Rights and costs associated with continuing and discontinuing service use
-   Service availability
-   Service performance
-   Data security and privacy
-   Disaster recovery processes
-   Data location
-   Data access
-   Data portability
-   Problem identification and resolution expectations
-   Change management processes
-   Dispute mediation processes
-   Exit strategy
****
# Cloud Service Terminology

Which cloud deployment model provides services to only one organization? (D4, L4.3.3) 

 A. Public
Incorrect. A public cloud is shared among many customers.
 B. Private
Correct. A private cloud includes cloud-based assets for a single organization.
 C. Hybrid
Incorrect. A hybrid cloud uses both public and private clouds together.

****
# Cloud Service Models

Which of the following cloud service models provides the most suitable environment for customers to build and operate their own software? (D4. L4.3.3)

 A. SaaS
Incorrect. SaaS provides access to software applications but not the equipment necessary for customers to build and operate their own software.
 B. IaaS
Incorrect. IaaS provides use of hardware and related equipment that is retained by the provider but does not allow customers to build and operate their own software in the most suitable way, since it would also require them to manage the operating systems as well.
 C. PaaS
Correct. PaaS typically provides a set of software building blocks and development tools, such as programming languages and supporting a run-time environment, that facilitate the construction of high-quality, scalable applications.
 D. SLA
Incorrect. SLA is a service-level agreement and is not a cloud service deployment model.


# Network Design

The objective of network design is to satisfy data communication requirements and result in efficient overall performance.

_Click each tab below to learn about several elements that are considered when planning for security in a network._ 

[Network Segmentation]()
Network segmentation involves controlling traffic among networked devices. Complete or physical network segmentation occurs when a network is isolated from all outside communications, so transactions can only occur between devices within the segmented network.
![[EDU-ELCC-70365-network_segmentation-v02.svg]]

[Demilitarized Zone (DMZ)]()

A DMZ is a network area that is designed to be accessed by outside visitors but is still isolated from the private network of the organization. The DMZ is often the host of public web, email, file and other resource servers.
![[EDU-ELCC-70370-dmz-v02.svg]]
![diagram of dimilitarized zone isolated from organization's workstations]

[Virtual Local Area Network (VLAN)]
VLANs are created by switches to logically segment a network without altering its physical topology.
![[EDU-ELCC-70375-techart-vlan-v02.svg]]



[Virtual Private Network (VPN)]()
A virtual private network (VPN) is a communication tunnel that provides point-to-point transmission of both authentication and data traffic over an untrusted network.
![[EDU-ELCC-70380-techart-vpn-v02.svg]]

[Defense in Depth]()
Defense in depth uses multiple types of access controls in literal or theoretical layers to help an organization avoid a monolithic security stance.
![[EDU-ELCC-70385-techart-DID-v01.svg]]


[Network Access Control (NAC)]()

Network access control (NAC) is a concept of controlling access to an environment through strict adherence to and implementation of security policy.

![[2023-03-03 08_16_07-Network Design.png]]


# Defense in Depth

Defense in depth uses a layered approach when designing the security posture of an organization. Think about a castle that holds the crown jewels. The jewels will be placed in a vaulted chamber in a central location guarded by security guards. The castle is built around the vault with additional layers of security—soldiers, walls, a moat (Fossato). The same approach is true when designing the logical security of a facility or system. Using layers of security will deter many attackers and encourage them to focus on other, easier targets. 

Defense in depth provides more of a starting point for considering all types of controls—administrative, technological, and physical—that empower insiders and operators to work together to protect their organization and its systems. 

Here are some examples that further explain the concept of defense in depth: 

-   Data: Controls that protect the actual data with technologies such as encryption, data leak prevention, identity and access management and data controls.
-   Application: Controls that protect the application itself with technologies such as data leak prevention, application firewalls and database monitors.
-   Host: Every control that is placed at the endpoint level, such as antivirus, endpoint firewall, configuration and patch management.
-   Internal network: Controls that are in place to protect uncontrolled data flow and user access across the organizational network. Relevant technologies include intrusion detection systems, intrusion prevention systems, internal firewalls and network access controls.
-   Perimeter: Controls that protect against unauthorized access to the network. This level includes the use of technologies such as gateway firewalls, honeypots, malware analysis and secure demilitarized zones (DMZs).
-   Physical: Controls that provide a physical barrier, such as locks, walls or access control.
-   Policies, procedures and awareness: Administrative controls that reduce insider threats (intentional and unintentional) and identify risks as soon as they appear.![[2023-03-03 11_56_54-Defense in Depth.png]]


# Zero Trust

>[!Zero trust]+ 
>Removing the design belief that the network has any trusted space. Security is managed at each possible level, representing the most granular asset. Microsegmentation of workloads is a tool of the model

networks are often microsegmented networks, with firewalls at nearly every connecting point. Zero trust encapsulates information assets, the services that apply to them and their security properties. This concept recognizes that once inside a trust-but-verify environment, a user has perhaps unlimited capabilities to roam around, identify assets and systems and potentially find exploitable vulnerabilities. Placing a greater number of firewalls or other security boundary control devices throughout the network increases the number of opportunities to detect a troublemaker before harm is done. Many enterprise architectures are pushing this to the extreme of microsegmenting their internal networks, which enforces frequent re-authentication of a user ID, as depicted in this image.  

Consider a rock music concert. By traditional perimeter controls, such as firewalls, you would show your ticket at the gate and have free access to the venue, including backstage where the real rock stars are. In a zero-trust environment, additional checkpoints are added. Your identity (ticket) is validated to access the floor level seats, and again to access the backstage area. Your credentials must be valid at all 3 levels to meet the stars of the show.  

Zero trust is an evolving design approach which recognizes that even the most robust access control systems have their weaknesses. It adds defenses at the user, asset and data level, rather than relying on perimeter defense. In the extreme, it insists that every process or action a user attempts to take must be authenticated and authorized; the window of trust becomes vanishingly small.  

While 
>[!microsegmentation]+
>Part of a zero trust strategy that breaks LANs into very small, highly localized zones using firewalls or similar technologies. At the limit, this places firewall at every connection point. 

adds internal perimeters, zero trust places the focus on the assets, or data, rather than the perimeter. Zero trust builds more effective gates to protect the assets directly rather than building additional or higher walls.
![[2023-03-03 13_47_56-Zero Trust.png]]


# Network Access Control (NAC)

An organization’s network is perhaps one of its most critical assets. As such, it is vital that we both know and control access to it, both from insiders (e.g., employees, contractors) and outsiders (e.g., customers, corporate partners, vendors). We need to be able to see who and what is attempting to make a network connection.

At one time, network access was limited to internal devices. Gradually, that was extended to remote connections, although initially those were the exceptions rather than the norm. This started to change with the concepts of bring your own device (BYOD) and Internet of Things (IoT).

Considering just IoT for a moment, it is important to understand the range of devices that might be found within an organization. They include heating, ventilation and air conditioning (HVAC) systems that monitor the ambient temperature and adjust the heating or cooling levels automatically or air monitoring systems, through security systems, sensors and cameras, right down to vending and coffee machines. Look around your own environment and you will quickly see the scale of their use.

Having identified the need for a NAC solution, we need to identify what capabilities a solution may provide. As we know, everything begins with a policy. The organization’s access control policies and associated security policies should be enforced via the NAC device(s). Remember, of course, that an access control device only enforces a policy and doesn’t create one.

The NAC device will provide the network visibility needed for access security and may later be used for incident response. Aside from identifying connections, it should also be able to provide isolation for noncompliant devices within a quarantined network and provide a mechanism to “fix” the noncompliant elements, such as turning on endpoint protection. In short, the goal is to ensure that all devices wishing to join the network do so only when they comply with the requirements laid out in the organization policies. This visibility will encompass internal users as well as any temporary users such as guests or contractors, etc., and any devices they may bring with them into the organization.

Let’s consider some possible use cases for NAC deployment: 

-   Medical devices
-   IoT devices
-   BYOD/mobile devices (laptops, tablets, smartphones)
-   Guest users and contractors

As we have established, it is critically important that all mobile devices, regardless of their owner, go through an onboarding process, ideally each time a network connection is made, and that the device is identified and interrogated to ensure the organization’s policies are being met.# Network Access Control (NAC)

An organization’s network is perhaps one of its most critical assets. As such, it is vital that we both know and control access to it, both from insiders (e.g., employees, contractors) and outsiders (e.g., customers, corporate partners, vendors). We need to be able to see who and what is attempting to make a network connection.

At one time, network access was limited to internal devices. Gradually, that was extended to remote connections, although initially those were the exceptions rather than the norm. This started to change with the concepts of bring your own device (BYOD) and Internet of Things (IoT).

Considering just IoT for a moment, it is important to understand the range of devices that might be found within an organization. They include heating, ventilation and air conditioning (HVAC) systems that monitor the ambient temperature and adjust the heating or cooling levels automatically or air monitoring systems, through security systems, sensors and cameras, right down to vending and coffee machines. Look around your own environment and you will quickly see the scale of their use.

Having identified the need for a NAC solution, we need to identify what capabilities a solution may provide. As we know, everything begins with a policy. The organization’s access control policies and associated security policies should be enforced via the NAC device(s). Remember, of course, that an access control device only enforces a policy and doesn’t create one.

The NAC device will provide the network visibility needed for access security and may later be used for incident response. Aside from identifying connections, it should also be able to provide isolation for noncompliant devices within a quarantined network and provide a mechanism to “fix” the noncompliant elements, such as turning on endpoint protection. In short, the goal is to ensure that all devices wishing to join the network do so only when they comply with the requirements laid out in the organization policies. This visibility will encompass internal users as well as any temporary users such as guests or contractors, etc., and any devices they may bring with them into the organization.

Let’s consider some possible use cases for NAC deployment: 

-   Medical devices
-   IoT devices
-   BYOD/mobile devices (laptops, tablets, smartphones)
-   Guest users and contractors

As we have established, it is critically important that all mobile devices, regardless of their owner, go through an onboarding process, ideally each time a network connection is made, and that the device is identified and interrogated to ensure the organization’s policies are being met.

![[2023-03-03 08_16_07-Network Design.png]]

# NAC Deeper Dive video
NacDeeperDive.mkv

Narrator: At its simplest form, Network Access Control, or NAC, is a way to prevent unwanted devices from connecting to a network. Some NAC systems allow for the installation of required software on the end user’s device to enforce device compliance to policy prior to connecting. A high-level example of a NAC system is hotel internet access. Typically, a user connecting to the hotel network is required to acknowledge the acceptable use policy before being allowed to access the internet. After the user clicks the acknowledge button, the device is connected to the network that enables internet access. Some hotels add an additional layer requiring the guest to enter a special password or a room number and guest name before access is granted. This prevents abuse by someone who is not a hotel guest and may even help to track network abuse to a particular user. A slightly more complex scenario is a business that separates employee BYOD devices from corporate-owned devices on the network. If the BYOD device is pre-approved and allowed to connect to the corporate network, the NAC system can validate the device using a hardware address or installed software, and even check to make sure the antivirus software and operating system software are up to date before connecting it to the network. Alternatively, if it is a personal device not allowed to connect to the corporate network, it can be redirected to the guest network for internet access without access to internal corporate resources.


# Network Segmentation (Demilitarized Zone (DMZ))

Network segmentation is also an effective way to achieve defense in depth for distributed or multi-tiered applications. The use of a demilitarized zone (DMZ), for example, is a common practice in security architecture. With a DMZ, host systems that are accessible through the firewall are physically separated from the internal network by means of secured switches or by using an additional firewall to control traffic between the web server and the internal network. Application DMZs (or semi-trusted networks) are frequently used today to limit access to application servers to those networks or systems that have a legitimate need to connect.
![[EDU-ELCC-70370-dmz-v02.svg]]


# DMZ Deeper Dive video

DMZDeeperDive.mkv

Narrator: A web front end server might be in the DMZ, but it might retrieve data from a database server that is on the other side of the firewall. 

For example, you may have a network where you manage your client’s personal information, and even if the data is encrypted or obfuscated by cryptography, you need to make sure the network is completely segregated from the rest of the network with some secure switches that only an authorized individual has access to. Only authorized personnel can control the firewall settings and control the traffic between the web server and the internal network. For example, in a hospital or a doctor’s office, you would have a segregated network for the patient information and billing, and on the other side would be the electronic medical records. If they are using a web-based application for medical record services, they would have a demilitarized zone or segmented areas. And perhaps even behind the firewall, they have their own specified server to protect the critical information and keep it segregated. 

It is worth noting at this point that while this course will not explore the specifics, some networks use a web application firewall (WAF) rather than a DMZ network. The WAF has an internal and an external connection like a traditional firewall, with the external traffic being filtered by the traditional or next generation firewall first. It monitors all traffic, encrypted or not, from the outside for malicious behavior before passing commands to a web server that may be internal to the network.

# Segmentation for Embedded Systems and IoT

An embedded system is a computer implemented as part of a larger system. The embedded system is typically designed around a limited set of specific functions in relation to the larger product of which it is a component. Examples of embedded systems include network-attached printers, smart TVs, HVAC controls, smart appliances, smart thermostats and medical devices. 

Network-enabled devices are any type of portable or nonportable device that has native network capabilities. This generally assumes the network in question is a wireless type of network, typically provided by a mobile telecommunications company. Network-enabled devices include smartphones, mobile phones, tablets, smart TVs or streaming media players (such as a Roku Player, Amazon Fire TV, or Google Android TV/Chromecast), network-attached printers, game systems, and much more. 

The Internet of Things (IoT) is the collection of devices that can communicate over the internet with one another or with a control console in order to affect and monitor the real world. IoT devices might be labeled as smart devices or smart-home equipment. Many of the ideas of industrial environmental control found in office buildings are finding their way into more consumer-available solutions for small offices or personal homes.  

Embedded systems and network-enabled devices that communicate with the internet are considered IoT devices and need special attention to ensure that communication is not used in a malicious manner. Because an embedded system is often in control of a mechanism in the physical world, a security breach could cause harm to people and property. Since many of these devices have multiple access routes, such as ethernet, wireless, Bluetooth, etc., special care should be taken to isolate them from other devices on the network. You can impose logical network segmentation with switches using VLANs, or through other traffic-control means, including MAC addresses, IP addresses, physical ports, protocols, or application filtering, routing, and access control management. Network segmentation can be used to isolate IoT environments.

![[EDU-ELCC-70535-techart-segmentation_embedded_systems_iot-v04.svg]]
# Segmentation for Embedded Systems and IoT Deeper Dive

Narrator: The characteristics that make embedded systems operate efficiently are also a security risk. Embedded systems are often used to control something physical, such as a valve for water, steam, or even oil. These devices have a limited instruction set and are often hardcoded or permanently written to a memory chip. For ease of operating the mechanical parts, the embedded system is often connected to a corporate network since and may operate using the TCP/IP protocol, yes, the same protocol that runs all over the internet. Therefore, it is feasible for anyone anywhere on the internet to control the opening and closing of a valve when the networks are fully connected. This is the primary reason for segmentation of these systems on a network. If these are segmented properly, a compromised corporate network will not be able to access the physical controls on the embedded systems. The other side of the embedded systems, which also applies to IoT devices, is the general lack of system updates when a new vulnerability is found. In the case of most embedded systems with the programming directly on the chips, it would require physical replacement of the chip to patch the vulnerability. For many systems, it may not be cost-effective to have someone visit each one to replace a chip, or manually connect to the chip to re-program it. We buy all these internet connected things because of the convenience. Cameras, light bulbs, speakers, refrigerators, etc. all bring some sort of convenience to our lives, but they also introduce risk. While the reputable mainstream brands will likely provide updates to their devices when a new vulnerability is discovered, many of the smaller companies simply don’t plan to do that as they seek to control the costs of a device. These devices, when connected to a corporate network, can be an easy internet-connected doorway for a cyber criminal to access a corporate network. If these devices are properly segmented, or separated, on the network from corporate servers and other corporate networking, a compromise on an IoT device or a compromised embedded system will not be able to access those corporate data and systems.

# Microsegmentation

The toolsets of current adversaries are polymorphic in nature and allow threats to bypass static security controls. Modern cyberattacks take advantage of traditional security models to move easily between systems within a data center. Microsegmentation aids in protecting against these threats. A fundamental design requirement of microsegmentation is to understand the protection requirements for traffic within a data center and traffic to and from the internet traffic flows. 

When organizations avoid infrastructure-centric design paradigms, they are more likely to become more efficient at service delivery in the data center and become apt at detecting and preventing advanced persistent threats.

# Microsegmentation Deeper Dive

Narrator: Some key points about microsegmentation: Microsegmentation allows for extremely granular restrictions within the IT environment, to the point where rules can be applied to individual machines and/or users, and these rules can be as detailed and complex as desired. For instance, we can limit which IP addresses can communicate to a given machine, at which time of day, with which credentials, and which services those connections can utilize. These are logical rules, not physical rules, and do not require additional hardware or manual interaction with the device (that is, the administrator can apply the rules to various machines without having to physically touch each device or the cables connecting it to the networked environment). This is the ultimate end state of the defense-in-depth philosophy; no single point of access within the IT environment can lead to broader compromise. This is crucial in shared environments, such as the cloud, where more than one customer’s data and functionality might reside on the same device(s), and where third-party personnel (administrators/technicians who work for the cloud provider, not the customer) might have physical access to the devices. Microsegmentation allows the organization to limit which business functions/units/offices/departments can communicate with others, in order to enforce the concept of least privilege. For instance, the Human Resources office probably has employee data that no other business unit should have access to, such as employee home address, salary, medical records, etc. Microsegmentation, like VLANs, can make HR its own distinct IT enclave, so that sensitive data is not available to other business entities, thus reducing the risk of exposure. In modern environments, microsegmentation is available because of virtualization and software-defined networking (SDN) technologies. In the cloud, the tools for applying this strategy are often called “virtual private networks (VPN)” or "security groups.” Even in your home, microsegmentation can be used to separate computers from smart TVs, air conditioning, and smart appliances which can be connected and can have vulnerabilities.

# Virtual Local Area Network (VLAN)

[Virtual local area networks](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/module_03/ch04_m03-Virtual_Local_Area_Network_(VLAN).html?d2lSessionVal=XGXVKYxmu6eSi5toaeWBGGtAJ&ou=9541&d2l_body_type=3#) (VLANs) allow network administrators to use switches to create software-based LAN segments, which can segregate or consolidate traffic across multiple switch ports. Devices that share a VLAN communicate through switches as if they were on the same Layer 2 network. This image shows different VLANs — red, green and blue — connecting separate sets of ports together, while sharing the same network segment (consisting of the two switches and their connection). Since VLANs act as discrete networks, communications between VLANs must be enabled. Broadcast traffic is limited to the VLAN, reducing congestion and reducing the effectiveness of some attacks. Administration of the environment is simplified, as the VLANs can be reconfigured when individuals change their physical location or need access to different services. VLANs can be configured based on switch port, IP subnet, MAC address and protocols.

VLANs do not guarantee a network’s security. At first glance, it may seem that traffic cannot be intercepted because communication within a VLAN is restricted to member devices. However, there are attacks that allow a malicious user to see traffic from other VLANs (so-called VLAN hopping). The VLAN technology is only one tool that can improve the overall security of the network environment.

![diagram of two VLANs connecting separate sets of ports together while sharing the same network segment](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/assets/EDU-ELCC-01455-techart-vlans_in_network-v01.svg?_&d2lSessionVal=XGXVKYxmu6eSi5toaeWBGGtAJ&ou=9541 "diagram of two VLANs connecting separate sets of ports together while sharing the same network segment")

# VLAN Segmentation

Narrator: VLANS are virtual separations within a switch and are used mainly to limit broadcast traffic. A VLAN can be configured to communicate with other VLANs or not, and may be used to segregate network segments. There are a few common uses of VLANs in corporate networks. The first is to separate Voice Over IP (VOIP) telephones from the corporate network. This is most often done to more effectively manage the network traffic generated by voice communications by isolating it from the rest of the network. Another common use of VLANs in a corporate network is to separate the data center from all other network traffic. This makes it easier to keep the server-to-server traffic contained to the data center network while allowing certain traffic from workstations or the web to access the servers. As briefly discussed earlier, VLANs can also be used to segment networks. For example, a VLAN can separate the payroll workstations from the rest of the workstations in the network. Routing rules can also be used to only allow devices within this Payroll VLAN to access the servers containing payroll information. Earlier, we also discussed Network Access Control (NAC). These systems use VLANs to control whether devices connect to the corporate network or to a guest network. Even though a wireless access controller may attach to a single port on a physical network switch, the VLAN associated with the device connection on the wireless access controller determines the VLAN that the device operates on and to which networks it is allowed to connect. Finally, in large corporate networks, VLANs can be used to limit the amount of broadcast traffic within a network. This is most common in networks of more than 1,000 devices and may be separated by department, location/building, or any other criteria as needed. The most important thing to remember is that while VLANs are logically separated, they may be allowed to access other VLANs. They can also be configured to deny access to other VLANs.

# Virtual Private Network (VPN)

A [virtual private network](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/module_03/ch04_m03-Virtual_Private_Network_(VPN).html?d2lSessionVal=XGXVKYxmu6eSi5toaeWBGGtAJ&ou=9541&d2l_body_type=3#) (VPN) is not necessarily an encrypted tunnel. It is simply a point-to-point connection between two hosts that allows them to communicate. Secure communications can, of course, be provided by the VPN, but only if the security protocols have been selected and correctly configured to provide a trusted path over an untrusted network, such as the internet. Remote users employ VPNs to access their organization’s network, and depending on the VPN’s implementation, they may have most of the same resources available to them as if they were physically at the office. As an alternative to expensive dedicated point-to-point connections, organizations use gateway-to-gateway VPNs to securely transmit information over the internet between sites or even with business partners.

# Network Design Terms

Which term describes a communication tunnel that provides point-to-point transmission of both authentication and data traffic over an untrusted network? (D4, L4.3.2) 

 A. VPN
Correct. A Virtual Private Network (VPN) describes a communication tunnel that provides point-to-point transmission of both authentication and data traffic over an untrusted network.

 B. Zero Trust
Incorrect. Zero trust is a concept that uses microsegmentation to protect network segments.

 C. DMZ
Incorrect. DMZ is a virtual segment usually defined by a firewall that contains less-trusted devices between the corporate network and the internet.

 D. None of the Above
Incorrect. A Virtual Private Network (VPN) describes a communication tunnel that provides point-to-point transmission of both authentication and data traffic over an untrusted network.