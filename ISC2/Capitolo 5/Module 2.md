# Module 2: Understand System Hardening

Domain D5.2.1

#### Module Objective

-   L5.2.1 Describe the concepts of configuration management.
- video SysHardening.mkv

Manny: With so much data to work with, and so many different software applications required to handle it, how do companies keep track of everything? Tasha: It's a challenge all right, that's why we need configuration management. It's part of cybersecurity in that it protects the confidentiality, integrity, and availability of data by making sure that only authorized and validated changes are made to a system. Every change also needs to be tested to make sure it doesn't cause any disruption to any other part of the system. Manny: I can understand that. It seems like every time we upgrade our computer systems at the high school, something else stops working. Tasha: Let's find out how cybersecurity professionals work to prevent that from happening

****
# Configuration Management Overview

>[!Configuration management]+ 
> A process and discipline used to ensure that the only changes made to a system are those that have been authorized and validated.

is a process and discipline used to ensure that the only changes made to a system are those that have been authorized and validated. It is both a decision-making process and a set of control processes. If we look closer at this definition, the basic configuration management process includes components such as identification, baselines, updates and patches.  

_Select each plus sign hotspot to learn more about each topic._![[Configuration Management Overview.png]]
##### Identification
Baseline identification of a system and all its components, interfaces and documentation.

##### Baseline
A security baseline is a minimum level of protection that can be used as a reference point. Baselines provide a way to ensure that updates to technology and architectures are subjected to the minimum understood and acceptable level of security requirements.

##### Change Control
An update process for requesting changes to a baseline, by means of making changes to one or more components in that baseline. A review and approval process for all changes. This includes updates and patches.

##### Verification and Audit
A regression and validation process, which may involve testing and analysis, to verify that nothing in the system was broken by a newly applied set of changes. An audit process can validate that the currently in-use baseline matches the sum total of its initial baseline plus all approved changes applied in sequence.


Effective use of configuration management gives systems owners, operators, support teams and security professionals another important set of tools they can use to monitor and oversee the configuration of the devices, networks, applications and projects of the organization. An organization may mandate the configuration of equipment through standards and baselines. The use of standards and baselines can ensure that network devices, software, hardware and endpoint devices are configured in a consistent way and that all such devices are compliant with the security baseline established for the organization. If a device is found that is not compliant with the security baseline, it may be disabled or isolated into a quarantine area until it can be checked and updated.

**Inventory Baselines Updates Patches **

**Inventory**
Making an inventory, catalog or registry of all the information assets that the organization is aware of (whether they already exist, or there’s a wish list or need to create or acquire them) is the first step in any asset management process. It requires that we locate and identify all assets of interest, including (and especially) the information assets:

You can’t protect what you don’t know you have.

It becomes even more challenging to keep that inventory, and its health and status with respect to updates and patches, consistent and current, day in and day out. It is, in fact, quite challenging to identify every physical host and endpoint, let alone gather the data from them all.

**Baseline**
A commercial software product, for example, might have thousands of individual modules, processes, parameter and initialization files or other elements. If any one of them is missing, the system cannot function correctly. The baseline is a total inventory of all the system’s components, hardware, software, data, administrative controls, documentation and user instructions.

Once controls are in place to mitigate risks, the baselines can be referenced. All further comparisons and development are measured against the baselines.

When protecting assets, baselines can be particularly helpful in achieving a minimal protection level of those assets based on value. Remember, if assets have been classified based on value, and meaningful baselines have been established for each of the classification levels, we can conform to the minimum levels required. In other words, if classifications such as high, medium and low are being used, baselines could be developed for each of our classifications and provide that minimum level of security required for each.

**Updates**
Repairs, maintenance actions and updates are frequently required on almost all levels of systems elements, from the basic infrastructure of the IT architecture on up through **operating systems**(_def: The software “master control application” that runs the computer. It is the first program loaded when the computer is turned on, and its main component, the kernel, resides in memory at all times. The operating system sets the standards for all application programs (such as the Web server) that run in the computer. The applications communicate with the operating system for most user interface and file management operations. NIST SP 800-44 Version 2 _), applications platforms, networks and user interfaces. Such modifications must be acceptance tested to verify that newly installed (or repaired) functionality works as required. They must also be regression tested to verify that the modifications did not introduce other erroneous or unexpected behaviors in the system. Ongoing security assessment and evaluation testing evaluates whether the same system that passed acceptance testing is still secure.

**Patches**
>[!Patch management]+ 
> The systematic notification, identification, deployment, installation and verification of operating system and application software code revisions. These revisions are known as patches, hot fixes, and service packs. Source: CNSSI 4009

mostly applies to software and hardware devices that are subject to regular modification. A **patch** (_def:  A software component that, when installed, directly modifies files or device settings related to a different software component without changing the version number or release details for the related software component. Source: ISO/IEC 19770-2_) is an update, upgrade or modification to a system or component. These patches may be needed to address a vulnerability or to improve functionality. The challenge for the security professional is maintaining all patches, since they can come at irregular intervals from many different vendors. Some patches are critical and should be deployed quickly, while others may not be as critical but should still be deployed because subsequent patches may be dependent on them. Standards such as the PCI DSS require organizations to deploy security patches within a certain time frame.

There are some issues with the use of patches. Many organizations have been affected by a flawed patch from a reputable vendor that affected system functionality. Therefore, an organization should test the patch before rolling it out across the organization. This is often complicated by the lack of a testing environment that matches the production environment. Few organizations have the budget to maintain a test environment that is an exact copy of production. There is always a risk that the testing will not always be able to test everything, and problems may appear in production that were not apparent in the test environment. To the extent possible, patches should be tested to ensure they will work correctly in production.

If the patch does not work or has unacceptable effects, it might be necessary to roll back to a previous (pre-patch) state. Typically, the criteria for rollback are previously documented and would automatically be performed when the rollback criteria were met.


Many vendors offer a patch management solution for their products. These systems often have certain automated processes, or unattended updates, that allow the patching of systems without interaction from the administrator. The risk of using unattended patching should be weighed against the risk of having unpatched systems in the organization’s network. Unattended (or automated) patching might result in unscheduled outages as production systems are taken offline or rebooted as part of the patch process.
****
# The Risks of Change
video: RiskOfChange.mkv

Narrator: You have to make sure you have a robust change management process and make sure you test in model environments before you make any change in a production or live environment. Even with extensive planning and testing, there are sometimes unintended consequences, so you must make sure there is a rollback plan. A rollback is restoring the system to the state it was in before the change was made. To the point where we know it was working properly before we introduced changes into the environment. We need to make sure we review and test all the patches and can restore the previous configuration. Maintaining a separate testing environment can be a logistical challenge for many organizations; as such, many do not have separate production and testing environments to properly vet all patches and system updates. In this case, they may rely on vendor third party testing to certify a new software release based on a generic set of data. The rollback plan is important in all environments, but it is absolutely critical in those who are unable to fully test a change.

fine Modulo 2




