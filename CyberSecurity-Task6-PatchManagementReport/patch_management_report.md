TASK 6: Research Report — The Importance of Patch Management
Topic: Patch management and cybersecurity risk reduction
Date: 9 November 2026
1. Introduction
Patch management is the organized process of identifying, obtaining, testing, installing and checking software or firmware updates. A patch is a change released by a developer or vendor to fix a security weakness, correct an error or improve the reliability of a system. Patches may apply to operating systems, applications, servers, network equipment, databases and other connected devices.

Patch management is an important part of the vulnerability management lifecycle. A vulnerability is a weakness that could be used to affect the confidentiality, integrity or availability of a system. Organisations first need to discover which technology they use and identify its weaknesses. They then assess the level of risk, decide how to address it and apply an appropriate fix. Installing a patch is often the main way to remove a known software weakness, while verification confirms that the fix worked. NIST describes enterprise patch management as identifying, prioritising, acquiring, installing and verifying patches, updates and upgrades [1].

Unpatched systems create an attack surface because attackers can target weaknesses that remain present after a security fix has become available. A computer connected to the internet, an exposed server or an old application can give an attacker an opportunity to enter an organisation's network. Good patch management reduces these opportunities, although it must be supported by other controls such as secure configuration, access control, backups and monitoring.
2. Why Security Patches Matter
2.1 How vulnerabilities are discovered and reported
Software vulnerabilities may be discovered by the developers who created the software, independent security researchers, customers, penetration testers or criminals. Responsible researchers normally report a weakness to the vendor or an authorised vulnerability-coordination team so that it can be investigated and fixed before details are widely used by attackers. Vendors may then publish a security advisory and release a patch or other mitigation.

A publicly disclosed vulnerability may receive a Common Vulnerabilities and Exposures (CVE) identifier. A CVE ID is a standard reference number that helps security teams, vendors and researchers refer to the same vulnerability. The CVE Program identifies, defines and catalogues publicly disclosed cybersecurity vulnerabilities [2]. For example, CVE-2017-5638 identifies the Apache Struts vulnerability involved in the 2017 Equifax breach.

The Common Vulnerability Scoring System (CVSS) is used to describe the technical severity of a vulnerability. CVSS version 4.0 produces a score from 0.0 to 10.0 and considers factors such as the vulnerability's technical characteristics, threat conditions and the environment in which it exists. The qualitative ratings are None, Low, Medium, High and Critical [3]. A high score is a useful warning, but it should not be the only factor used to decide patch order. Organisations should also consider whether attackers are already exploiting the weakness, whether the affected system is exposed to the internet and how important the system is to the business.

The National Vulnerability Database (NVD), maintained by NIST, provides additional information about publicly known vulnerabilities. CISA's Known Exploited Vulnerabilities (KEV) Catalog identifies vulnerabilities for which there is evidence of exploitation in the wild. CISA recommends that organisations use the KEV Catalog to prioritise remediation because those weaknesses are already being used by attackers [4].
2.2 Why unpatched systems are attractive targets
When a vendor releases a security patch, the weakness may become more widely understood. Attackers can study the security advisory, develop or reuse exploit code and search for systems that have not installed the update. This creates a race between defenders applying the fix and attackers attempting to exploit the weakness. An unpatched system may remain vulnerable even when the organisation knows that a fix exists.

The scale of this problem is shown in Verizon's 2026 Data Breach Investigations Report. The report found that exploitation of software vulnerabilities was the initial entry point in 31% of breaches analysed, making it the leading initial access method in that report [5]. This does not mean that every such breach was caused by a missing patch, but it demonstrates how often attackers take advantage of software weaknesses.
2.3 Real-world examples
Example 1: WannaCry ransomware and Eternal Blue (2017)
In March 2017, Microsoft released security update MS17-010 to fix serious vulnerabilities in the Windows Server Message Block (SMB) service [6]. One of the weaknesses was later exploited using a tool known as EternalBlue. In May 2017, the WannaCry ransomware spread across many countries, encrypting files and disrupting organisations. CERT-EU reported that the attack used the SMB vulnerability and noted that Microsoft had released the relevant update on 14 March 2017, before the ransomware outbreak on 12 May 2017 [7]. Systems that had installed the security update were protected against the EternalBlue exploitation used by WannaCry. The incident showed how delaying patches can allow malware to spread through connected systems.
Example 2: Equifax data breach (2017)
The 2017 Equifax breach involved an unpatched vulnerability in Apache Struts, identified as CVE-2017-5638. The Apache Software Foundation released a fix on 7 March 2017 [8]. A U.S. Government Accountability Office report found that Equifax did not properly identify the vulnerable online dispute portal. The security notification was sent internally, but the distribution list was out of date and did not reach the staff responsible for applying the patch. A later scan also failed to detect the weakness [9]. Attackers accessed personal information relating to approximately 147 million people. The breach demonstrates why organisations need accurate asset inventories, clear responsibility for patching and reliable verification—not simply a written patching policy.

These incidents show that patches are not optional housekeeping. They are a way of removing known weaknesses before attackers can use them.
3. Consequences of Not Patching
Failure to install security updates can affect an organization in several ways:
1. Data breaches and loss of privacy: Attackers may use a known weakness to access customer records, employee information, passwords, financial details or confidential business documents. Exposed data can lead to identity theft, fraud and loss of customer trust.
2. Ransomware and service disruption: Malware may exploit vulnerable systems, encrypt files or interrupt essential services. Recovery can require restoring backups, rebuilding devices and investigating the incident. Organisations may also lose income while services are unavailable.
3. Financial costs: Costs can include investigation, legal advice, recovery, customer notification, system replacement, increased insurance costs and lost business. IBM's 2026 Cost of a Data Breach Report gives the global average cost of a data breach as US$4.99 million [10]. This figure covers data breaches generally; it is not a cost estimate for patch-related incidents alone.
4. Compliance and contractual problems: Organizations that fail to protect personal or commercially sensitive information may breach data-protection requirements, industry rules or contractual security obligations. The consequences depend on the relevant law and the facts of the incident. For example, the European Commission explains that serious GDPR infringements can attract fines of up to €20 million or 4% of an organisation's total annual worldwide turnover, whichever is applicable under the regulation [11].
5. Penalties and reputational damage: The Equifax settlement following its 2017 breach provided for at least US$575 million and potentially up to US$700 million in monetary relief and penalties [12]. The settlement included consumer compensation and civil penalties, showing how expensive failures in data security can become. A breach can also cause customers and business partners to lose confidence in an organisation.
The statistics above come from global research and examples in other jurisdictions. They should be treated as indicators of the possible scale of cyber risk; actual costs and legal penalties vary by organisation, country and incident.
4. The Patch Management Lifecycle
An effective patch management process should be repeated continuously. The main stages are discovery, assessment, testing, deployment and verification.
4.1 Discovery
The organization identifies all devices, operating systems, applications, servers, network equipment and cloud services that it owns or manages. It records software versions, system owners and business functions. This inventory is important because an organisation cannot patch a device or application it does not know exists. Automated asset discovery and vulnerability-scanning tools can help identify missing updates and unsupported software.
4.2 Assessment and prioritization
The IT or security team reviews available vendor advisories, CVE records, CVSS scores and the CISA KEV Catalog. It checks which systems are affected and considers the seriousness of the weakness, evidence of active exploitation, internet exposure, sensitivity of the data and importance of the system. Critical vulnerabilities that are actively exploited or affect internet-facing systems should normally receive urgent attention. Lower-risk updates can be scheduled according to the organisation's approved patching timetable.
4.3 Testing
Before a patch is installed across the whole organization, it should be tested in a controlled environment or on a small pilot group. The team checks whether the update installs correctly and whether important applications, integrations and business processes continue to work. Backups and a rollback plan should be prepared in case the update causes problems. Testing should be proportionate to the risk: an actively exploited critical vulnerability may require emergency deployment with a shorter testing window.
4.4 Deployment
After approval, the patch is installed on the affected systems. Organisations can use centralised patch-management tools, endpoint-management platforms or approved automation to distribute updates. Deployment should follow a schedule that states who is responsible, which systems are covered and the deadline for each risk category. Emergency patches may need to be deployed outside normal maintenance hours. Systems that cannot be patched immediately should receive temporary protective measures, such as restricting network access, disabling the vulnerable service or isolating the device.
4.5 Verification and review
The team confirms that the patch was successfully installed and that the system is running the expected software version. It should repeat vulnerability scans or use endpoint-management reports to identify devices that were missed or failed to update. The team also checks that services are working normally, records any exceptions and updates the asset inventory. Failed installations must be investigated and rescheduled. Verification closes the patching cycle and provides evidence that the weakness has been addressed.
5. Seven-Step Patch Management Checklist for Organisations
The following checklist provides a practical, prioritised approach:
1. Maintain a complete asset inventory. Record every organisation-owned device, application, server, cloud service and software version, along with its owner and business importance.
2. Monitor trusted vulnerability information. Subscribe to vendor security advisories and monitor CVE records, NVD information and the CISA KEV Catalog for vulnerabilities affecting the organisation's technology.
3. Prioritise using risk, not just release date. Give urgent attention to vulnerabilities being actively exploited, internet-facing systems, critical business services and systems containing sensitive information. Use CVSS as one input, not the only decision.
4. Set clear patching deadlines and responsibilities. Approve a policy that defines who reviews, tests and installs patches, and sets shorter deadlines for critical or actively exploited vulnerabilities.
5. Test important updates safely. Use a test environment or pilot group, check application compatibility, back up important data and prepare a rollback plan. Do not allow testing to create unnecessary delays for urgent security fixes.
6. Deploy updates and manage exceptions. Use centralised tools and automation where possible. Track successful installations, failed updates and devices that are temporarily unable to receive a patch. Apply compensating controls to systems awaiting remediation.
7. Verify, document and improve. Run follow-up scans, confirm software versions, record evidence of completion and review patching performance. Investigate missed devices and use the findings to improve the next cycle.
6. Challenges Organisations Face and How to Overcome Them
6.1 Legacy and unsupported systems
Some organisations depend on older systems that no longer receive security updates. Replacing them may be expensive or difficult because essential applications may only work on the old platform. Organisations should plan a gradual replacement, confirm vendor support status and prioritise systems that are exposed or hold sensitive information. Where replacement cannot happen immediately, isolate the legacy system, restrict access, disable unnecessary services and monitor it closely. These controls reduce risk but do not provide the same protection as a supported and patched system.
6.2 Downtime and business disruption
Installing updates can require restarts or temporary service interruptions. Organisations may delay patches because they want to avoid disrupting customers or employees. To address this, IT teams should schedule routine maintenance during low-use periods, communicate planned downtime and use redundancy or failover systems where possible. Emergency security patches should have a separate fast-track process so that serious weaknesses are not left exposed until the next routine maintenance window.
6.3 Compatibility and testing requirements
A patch may affect an older application, a device driver or a connection between systems. Testing reduces the chance of this happening in production, but long testing periods can leave a known vulnerability open. Organisations should maintain representative test environments, use pilot deployments and classify patches by risk. When exploitation is already occurring, testing should be focused and time-limited, with backups and rollback arrangements ready.
6.4 Limited staff, budgets and visibility
Small organisations may not have enough cybersecurity staff or tools to monitor every asset and update. Cloud services, remote devices and software installed by different departments can also make it difficult to know what needs patching. Organisations can improve visibility through centralised device management, automated inventory and vulnerability-scanning tools. They should assign clear ownership and concentrate limited resources on the systems and vulnerabilities that pose the greatest risk.
6.5 Missed devices and failed installations
A patch may fail because a device is offline, lacks storage space, has an incompatible configuration or is not included in the deployment group. A deployment notification alone does not prove that a system is secure. Organisations should use follow-up reports and vulnerability scans, identify devices that remain vulnerable and assign someone to resolve each exception.
7. Conclusion
Patch management is a basic but essential cybersecurity activity. It helps organisations remove known software weaknesses before criminals can exploit them. The WannaCry and Equifax incidents show that a security update is only useful when an organisation knows which systems are affected, assigns responsibility, applies the fix and checks that it has worked.

Organisations should treat patching as a continuous risk-management process rather than an occasional IT task. A complete asset inventory, risk-based prioritisation, controlled testing, timely deployment and verification can significantly reduce the chance of ransomware, data breaches and service disruption. Although patching cannot prevent every cyberattack, an organised patch management strategy reduces avoidable exposure and strengthens the organisation's overall security.
8. References
[1] Souppaya, M. and Scarfone, K. (2022). Guide to Enterprise Patch Management Planning: Preventive Maintenance for Technology. NIST Special Publication 800-40 Rev. 4. National Institute of Standards and Technology. https://csrc.nist.gov/pubs/sp/800/40/r4/final

[2] CVE Program. (n.d.). Common Vulnerabilities and Exposures (CVE). https://www.cve.org/

[3] Forum of Incident Response and Security Teams (FIRST). (2023). Common Vulnerability Scoring System Version 4.0: Specification Document. https://www.first.org/cvss/specification-document

[4] Cybersecurity and Infrastructure Security Agency (CISA). (n.d.). Reducing the Significant Risk of Known Exploited Vulnerabilities. https://www.cisa.gov/known-exploited-vulnerabilities-catalog

[5] Verizon. (2026). 2026 Data Breach Investigations Report: Vulnerability exploitation top breach entry point. https://www.verizon.com/about/news/breach-industry-wide-dbir-finds

[6] Microsoft. (2017, March 14). Microsoft Security Bulletin MS17-010 — Critical: Security Update for Microsoft Windows SMB Server. https://learn.microsoft.com/en-us/security-updates/securitybulletins/2017/ms17-010

[7] CERT-EU. (2017, May 22). Security Advisory 2017-012: WannaCry Ransomware Campaign Exploiting SMB Vulnerability. https://cert.europa.eu/publications/security-advisories/2017-012/

[8] The Apache Software Foundation. (2017, September 9). Response to Questions from the U.S. House Committee on Energy and Commerce Regarding Equifax Data Breach. https://news.apache.org/foundation/entry/responses-to-questions-from-us

[9] U.S. Government Accountability Office. (2018). Data Protection: Actions Taken by Equifax and Federal Agencies in Response to the 2017 Breach (GAO-18-559). https://www.gao.gov/products/gao-18-559

[10] IBM. (2026). Cost of a Data Breach Report 2026. https://www.ibm.com/reports/data-breach

[11] European Commission. (n.d.). Enforcement and sanctions under the General Data Protection Regulation. https://commission.europa.eu/law/law-topic/data-protection/information-business-and-organisations/enforcement-and-sanctions_en

[12] Federal Trade Commission. (2019, July 22). Equifax to Pay $575 Million as Part of Settlement with FTC, CFPB, and States Related to 2017 Data Breach. https://www.ftc.gov/news-events/news/press-releases/2019/07/equifax-pay-575-million-part-settlement-ftc-cfpb-states-related-2017-data-breach
