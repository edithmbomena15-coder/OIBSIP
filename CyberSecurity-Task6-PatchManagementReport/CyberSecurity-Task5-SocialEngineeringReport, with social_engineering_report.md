TASK 5: Research Report — Social Engineering Attacks
1. Introduction
Social engineering is the use of deception, impersonation, or psychological manipulation to persuade people to reveal information, provide access, or perform an action that benefits an attacker. Instead of relying only on technical weaknesses, social engineering targets human behaviour—such as trust, curiosity, fear, urgency, and the desire to help.

Social engineering is an effective attack vector because people may make quick decisions under pressure, and attackers can imitate familiar organisations or colleagues. Security tools can reduce risk, but they cannot completely prevent a person from voluntarily sharing a password or approving a fraudulent request. Verizon’s 2024 Data Breach Investigations Report stated that 68% of breaches involved a non-malicious human element, such as a person being tricked or making an error. This figure refers to the report’s overall breach dataset and should not be interpreted as meaning every breach was caused by social engineering (Verizon, 2024). Verizon’s 2026 DBIR also identified phishing as the initial access vector in 16% of breaches in its dataset, while vulnerability exploitation was the leading initial access vector overall. These figures come from different report years and datasets, so they should be treated as separate findings rather than a direct trend comparison (Verizon, 2026).

The main attack types discussed in this report are phishing, pretexting, and baiting. Quid pro quo is also included as a bonus example.
2. Phishing
2.1 Definition and how it works
Phishing is a social engineering attack in which an attacker pretends to be a trusted person or organisation to trick a target into clicking a malicious link, opening an attachment, sharing credentials, or sending money. Messages may appear to come from a bank, employer, delivery company, university, or online service.

A typical phishing attack follows these steps:
1. The attacker chooses a target or group of targets.
2. The attacker creates a convincing email, text, or message, often using a familiar name or logo.
3. The message encourages the recipient to act quickly—for example, to “verify” an account or open an invoice.
4. The victim clicks a link, opens a file, or provides information.
5. The attacker uses the stolen information to access accounts, install malware, or commit fraud.
2.2 Types of phishing
- Spear phishing: A targeted message designed for a particular person or organisation. It may include details about the recipient’s job, colleagues, or current activities.
- Whaling: A targeted phishing attack aimed at senior executives or other high-value individuals, such as a CEO or finance director.
- Vishing (voice phishing): A scam carried out through phone calls or voice messages. The attacker may impersonate a bank employee, IT support worker, or government official.
- Smishing (SMS phishing): A phishing attempt sent through text messages. It may contain a fake delivery notice, account warning, or payment request.
2.3 Real-world case study: Twitter hack (2020)
In July 2020, attackers gained access to internal tools used by Twitter (now X) and took over a number of high-profile accounts. The compromised accounts included those belonging to public figures and companies. The attackers used the access to publish messages promoting a cryptocurrency scam.

Public reporting and Twitter’s investigation described a social engineering operation in which attackers targeted employees and obtained access to internal systems. The incident demonstrated that an attacker does not always need to break through a technical vulnerability: deceiving employees can provide a route to powerful internal tools. The case also showed how a single compromised account or internal system can affect many users and damage public trust (FBI, 2020; Twitter, 2020).
2.4 Four prevention recommendations for phishing
1. Check the sender and destination: Inspect the full email address and hover over links before opening them. Be cautious of misspellings, unexpected attachments, and unfamiliar domains.
2. Verify unusual requests independently: If a message requests a payment, password, or urgent action, contact the person or organisation using a known phone number or official website—not the details in the message.
3. Use phishing-resistant authentication: Enable multi-factor authentication (MFA), preferably passkeys or security keys where supported. MFA reduces the damage caused by stolen passwords, although some methods can still be targeted.
4. Report suspicious messages: Use the organisation’s reporting process and avoid forwarding suspicious attachments to colleagues. Security teams can investigate and block similar messages.
3. Pretexting
3.1 Definition
Pretexting is a social engineering technique in which an attacker invents a believable story or situation—a “pretext”—to gain a person’s trust and obtain information, access, or a particular action. The attacker may pretend to be a manager, supplier, customer, IT technician, auditor, or other trusted person.
3.2 How an attacker builds a false scenario
An attacker may first gather publicly available information about the target, such as their name, position, workplace, or colleagues. The attacker then creates a story that fits the target’s role. For example, a person pretending to be a senior manager might claim that a confidential payment must be made immediately. The attacker uses authority, urgency, secrecy, or familiarity to discourage the victim from checking the request.
3.3 Real-world case study: FACC CEO fraud (2016)
In 2016, Austrian aircraft-parts manufacturer FACC disclosed that it had been affected by a “CEO fraud” attack. Attackers impersonated the company’s chief executive and persuaded an employee to transfer funds as part of a supposed confidential business transaction. The company reported a loss of approximately €50 million. FACC later announced personnel consequences involving senior management.

This incident is an example of pretexting because the attackers relied on a fabricated business scenario and the authority associated with the CEO’s identity. Reuters reported that the company initially disclosed a fraud of around €50 million, later recording a €41.9 million charge after blocking €10.9 million from being transferred. It demonstrates why financial requests must be verified through a separate, established process rather than accepted solely because they appear to come from a senior person (Nasralla, 2016).
3.4 Three prevention measures for pretexting
1. Use independent verification: Confirm sensitive requests—especially changes to bank details, payments, password resets, or confidential information—through a known contact method.
2. Apply separation of duties: Require a second authorised person to approve significant payments or sensitive account changes. A single employee should not be able to initiate and approve the same transaction.
3. Limit information shared publicly: Avoid publishing unnecessary internal details, staff information, schedules, or procedures. Train employees to recognise impersonation and pressure tactics.
4. Baiting
4.1 Definition
Baiting is a social engineering attack that offers something attractive or uses curiosity to persuade a person to take an unsafe action. The “bait” may be a free download, a prize, a tempting offer, or a physical device such as a USB drive.
4.2 Physical and digital baiting
- Physical baiting: An attacker leaves a device—often a USB drive labelled with an interesting name—in a place where someone may find it. A curious person may connect it to a work computer, potentially introducing malicious software.
- Digital baiting: An attacker advertises a free film, software tool, game, document, or other download. The file or website may install malware, steal credentials, or redirect the user to a fraudulent page.
Baiting relies mainly on curiosity, greed, or the expectation of receiving something useful or valuable.
4.3 Case study: University of Illinois dropped-USB experiment
A stronger example of physical baiting comes from a 2016 study by researchers from the University of Illinois Urbana-Champaign and the University of Michigan, published at the IEEE Symposium on Security and Privacy. The researchers dropped 297 USB flash drives around a university campus. The paper reports that 290 drives (about 98%) were picked up, and 135 drives (about 45% of all 297 dropped) had files opened. The first drive was connected in less than six minutes. The researchers found that people often connected the drives because they wanted to identify and return the owner’s device—not simply because they were careless (Tischer et al., 2016).

The experiment illustrates how an unknown USB drive can act as bait: curiosity or helpfulness may lead someone to connect a device that could contain malicious files. The researchers used a controlled tracking method and did not automatically run malware; therefore, the study demonstrates user behaviour and exposure, not that the experiment infected participants’ computers.

Related example: Stuxnet, discovered in 2010, was sophisticated malware that could spread through removable media and targeted industrial control systems associated with Iran’s nuclear programme. It is useful as an example of the risk posed by removable media, but it was not simply a campus-style USB baiting campaign (Symantec, 2011).
4.4 Three prevention measures for baiting
1. Never connect unknown USB devices: Give found or unsolicited storage devices to the IT or security team. Do not plug them into personal or work computers.
2. Control removable media: Organisations should disable autorun where appropriate, restrict USB use, and use endpoint protection to scan permitted devices.
3. Download from trusted sources: Obtain software from official websites or approved company repositories. Avoid suspicious “free” downloads, unexpected prizes, and offers that seem too good to be true.
5. Bonus: Quid Pro Quo
Quid pro quo means “something for something.” In a social engineering attack, the attacker offers a service, benefit, or reward in exchange for information or access. For example, someone may pretend to be IT support and offer to fix a user’s computer in exchange for the user’s password. The attacker may also offer a gift or payment for completing a task that exposes company information.

Prevention: Employees should never disclose passwords to support staff, and IT support should follow approved identity-verification procedures. Organisations should also ensure that legitimate support teams do not ask users to share credentials.
6. Comparison of Social Engineering Attacks
Attack type	Primary target	Psychological lever exploited	Best countermeasure
Phishing	Email, message, or online-service users	Trust, urgency, fear	Verify links and requests; report suspicious messages
Spear phishing	A specific employee or organisation	Personalisation and familiarity	Verify requests independently and use MFA
Whaling	Executives and senior decision-makers	Authority, urgency, confidentiality	Strong approval controls and independent verification
Vishing	People reached by phone	Trust in a voice or claimed institution	Call back using a verified official number
Smishing	Mobile phone users	Urgency and convenience	Avoid unexpected links; use official apps or websites
Pretexting	Employees, finance teams, help desks	Authority, trust, pressure	Identity verification and separation of duties
Baiting	People tempted by a device, offer, or download	Curiosity, greed, reward	Do not use unknown media; download only from trusted sources
Quid pro quo	Users seeking help or a benefit	Reciprocity and expectation of reward	Approved support processes; never share passwords


7. Organisational Recommendations: Five-Point Employee Security Awareness Checklist
Organisations should use a continuing awareness programme rather than relying on a single annual presentation.
1. Provide regular training: Teach employees to identify phishing, impersonation, suspicious calls, unsafe downloads, and unknown USB devices.
2. Use realistic practice exercises: Conduct authorised phishing simulations and discuss the warning signs with employees in a supportive manner.
3. Create a clear reporting process: Make it easy to report suspicious emails, messages, calls, and physical devices. Respond quickly and provide feedback.
4. Establish verification and approval procedures: Require independent checks for payments, bank-detail changes, credential resets, and requests for sensitive information.
5. Review and improve the programme: Track reports, simulation results, and recurring mistakes. Update training when new attack methods appear, and avoid blaming employees who report mistakes promptly.
8. Conclusion
Social engineering attacks exploit human behaviour to gain information, access, or money. Phishing commonly uses deceptive messages, pretexting relies on a believable false story, and baiting uses curiosity or an attractive offer. Real-world incidents such as the 2020 Twitter hack and the FACC CEO fraud show that these attacks can cause significant financial and reputational damage. Organisations can reduce the risk by combining employee awareness, independent verification, strong authentication, restricted access, and clear reporting procedures. Cybersecurity is therefore not only a technical responsibility; it is also a shared responsibility among employees, management, and IT teams.
9. References
- Cybersecurity and Infrastructure Security Agency (CISA), National Security Agency (NSA), Federal Bureau of Investigation (FBI), & Multi-State Information Sharing and Analysis Center (MS-ISAC). (2023; updated 2025). Phishing Guidance: Stopping the Attack Cycle at Phase One. https://www.cisa.gov/resources-tools/resources/phishing-guidance-stopping-attack-cycle-phase-one
- Federal Bureau of Investigation, Internet Crime Complaint Center (IC3). (2024, April 11). Cyber Criminals Target Victims Using Social Engineering Techniques. https://www.ic3.gov/PSA/2024/PSA240411
- French, L. (2026, May 20). Verizon DBIR 2026: Vulnerability exploits top initial access as patching coverage falls. SC Media. https://www.scworld.com/news/verizon-dbir-2026-vulnerability-exploits-top-initial-access-as-patching-coverage-falls
- Nasralla, S. (2016, May 25). Austria’s FACC, hit by cyber fraud, fires CEO. Reuters. https://finance.yahoo.com/news/austrias-facc-hit-cyber-fraud-091143191.html
- New York State Department of Financial Services (NYDFS). (2020, October 14). Report on Investigation of Twitter’s July 15, 2020 Cybersecurity Incident and the Implications for Election Security. https://www.dfs.ny.gov/reports-and-publications/other-reports/Twitter_Report
- Symantec. (2011). W32.Stuxnet dossier. https://docs.broadcom.com/doc/security-response-w32-stuxnet-dossier-11-en
- Tischer, M., Durumeric, Z., Foster, S., Duan, S., Mori, A., Bursztein, E., & Bailey, M. (2016). Users really do plug in USB drives they find. 2016 IEEE Symposium on Security and Privacy. https://ieeexplore.ieee.org/abstract/document/7546509
- Twitter. (2020, July 18; updated July 30). An update on our security incident. https://blog.x.com/en/company/an-update-on-our-security-incident
- U.S. Department of Health and Human Services, Office for Civil Rights. (2024, October). Social Engineering: Searching for Your Weakest Link. https://www.hhs.gov/hipaa/for-professionals/security/guidance/cybersecurity-newsletter-october-2024/index.html
- Verizon. (2024). 2024 Data Breach Investigations Report. https://www.verizon.com/business/resources/reports/2024/2024-dbir-data-breach-investigations-report.pdf
- Verizon. (2026). 2026 Data Breach Investigations Report. https://www.verizon.com/business/resources/T1e0/reports/2026-dbir-data-breach-investigations-report.pdf
- National Security Agency (NSA). (2023, October 18). How to Protect Against Evolving Phishing Attacks. https://www.nsa.gov/Press-Room/Press-Releases-Statements/Press-Release-View/Article/3560788/how-to-protect-against-evolving-phishing-attacks/
