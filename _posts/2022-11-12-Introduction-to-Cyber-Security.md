---
title: "TryHackMe - Introduction to Cyber Security"
last_modified_at: 2022-11-12
categories:
  - THM
tags:
  - THM
  - TryHackMe
---

![image](https://user-images.githubusercontent.com/66146701/201733926-d099ce02-1d7f-4828-8d31-405a75bc4e0e.png)

Cyber Security is a huge topic, and it can be challenging to know where to start. This path will give you a hands-on introduction to different areas within cyber, including:

- Careers in Cyber Security
- Offensive Security; hacking your first application
- Defensive Security; defending against a live cyber attack
- Exploring security topics in the industry

Completing this learning path will give you the knowledge to kick start your cyber journey.

# Introduction to Cyber Security

Understand what is offensive and defensive security, and learn about careers available in cyber.

## Intro to Offensive Security

Hack your first website (legally in a safe environment) and experience an ethical hacker's job.

`GoBuster` to brute-force FakeBank's website to find hidden directories and pages.

```jsx
gobuster -u http://fakebank.com/ -w wordlist.txt dir
```

![image](https://user-images.githubusercontent.com/66146701/202235125-e89df0ad-c9f1-42b3-a092-28c1e6d23ef3.png)

GoBuster will have told you the pages it found in the list of page/directory names (indicated by Status: 200).

Transfer $2000 from the bank account 2276, to your account (account number 8881).

![image](https://user-images.githubusercontent.com/66146701/202235184-313dd130-ae2f-4d78-96ad-e4280fc0ac10.png)

![image](https://user-images.githubusercontent.com/66146701/202235247-2948adac-e097-4e7c-b504-9c132afffac2.png)


### What is Offensive Security?

`offensive security` is the process of breaking into computer systems, exploiting software bugs, and finding loopholes in applications to gain unauthorized access to them. 

To beat a hacker, you need to behave like a hacker, finding vulnerabilities and recommending patches before a cyber criminal does.

On the flip side, there is also `defensive security`, which is the process of protecting an organization's network and computer systems by analyzing and securing any potential digital threats. 

In a defensive cyber role, you could be investigating infected computers or devices to understand how it was hacked, tracking down cyber-criminals, or monitoring infrastructure for malicious activity.

### Careers in cyber security

short description of a few offensive security roles:

- Penetration Tester - Responsible for testing technology products for finding exploitable security vulnerabilities.
- Red Teamer - Plays the role of an adversary, attacking an organization and providing feedback from an enemy's perspective.
- Security Engineer - Design, monitor, and maintain security controls, networks, and systems to help prevent cyberattacks.

## Intro to Defensive Security

Introducing defensive security and related topics, such as threat intelligence, SOC, DFIR, and SIEM.

### Introduction to Defensive Security

Offensive security focuses on one thing: breaking into systems. Breaking into systems might be achieved through exploiting bugs, abusing insecure setups, and taking advantage of unenforced access control policies, among other things. Red teams and penetration testers specialize in offensive security.

Defensive security is somewhat the opposite of offensive security, as it is concerned with two main tasks:

1. Preventing intrusions from occurring
2. Detecting intrusions when they occur and responding properly 

Blue teams are part of the defensive security landscape.

![image](https://user-images.githubusercontent.com/66146701/202235335-dfcc678a-e692-4c32-8052-1df73f38172f.png)

Some of the tasks that are related to defensive security include:

- **User cyber security awareness:** Training users about cyber security helps protect against various attacks that target their systems.
- **Documenting and managing assets:** We need to know the types of systems and devices that we have to manage and protect properly.
- **Updating and patching systems:** Ensuring that computers, servers, and network devices are correctly updated and patched against any known vulnerability (weakness).
- **Setting up preventative security devices:** firewall and intrusion prevention systems (IPS) are critical components of preventative security. Firewalls control what network traffic can go inside and what can leave the system or network. IPS blocks any network traffic that matches present rules and attack signatures.
- **Setting up logging and monitoring devices:** Without proper logging and monitoring of the network, it won’t be possible to detect malicious activities and intrusions. If a new unauthorized device appears on our network, we should be able to know.

There is much more to defensive security, and the list above only covers a few common topics.

- Security Operations Center (SOC)
- Threat Intelligence
- Digital Forensics and Incident Response (DFIR)
- Malware Analysis

![image](https://user-images.githubusercontent.com/66146701/202235391-b84cfbc9-8a9b-42d0-8e10-34c832e1ef7f.png)


## Areas of Defensive Security

### Security Operations Center (SOC)

A *Security Operations Center* (SOC) is a team of cyber security professionals that monitors the network and its systems to detect malicious cyber security events. Some of the main areas of interest for a SOC are:

- **Vulnerabilities:** Whenever a system vulnerability (weakness) is discovered, it is essential to fix it by installing a proper update or patch. When a fix is not available, the necessary measures should be taken to prevent an attacker from exploiting it. Although remediating
vulnerabilities is of vital interest to a SOC, it is not necessarily assigned to them.
- **Policy violations:** We can think of a security policy as a set of rules required for the protection of the network and systems. For example, it might be a policy violation if users start uploading
confidential company data to an online storage service.
- **Unauthorized activity:** Consider the case where a user’s login name and password are stolen, and the attacker uses them to log into the network. A SOC needs to detect such an event and block it as soon as possible before further damage is done.
- **Network intrusions:** No matter how good your security is, there is always a chance for an intrusion. An intrusion can occur when a user clicks on a malicious link or when an attacker exploits a public server. Either way, when an intrusion occurs, we must detect it as soon as
possible to prevent further damage.

Security operations cover various tasks to ensure protection; one such task is threat intelligence.

![image](https://user-images.githubusercontent.com/66146701/202235454-f4b6b5d1-212b-44c8-afd8-d472a1edbf27.png)


### Threat Intelligence

In this context, *intelligence* refers to information you gather about actual and potential enemies. A *threat* is any action that can disrupt or adversely affect a system. Threat intelligence aims to gather information to help the company better prepare against potential adversaries. The purpose would be to achieve a *threat-informed defense*. Different companies have different adversaries. Some adversaries might seek to steal customer data from a mobile operator; however, other adversaries are interested in halting the production in a petroleum refinery. Example adversaries include a 
nation-state cyber army working for political reasons and a ransomware group acting for financial purposes. Based on the company (target), we can expect adversaries.

![image](https://user-images.githubusercontent.com/66146701/202235514-0c6f447a-11a9-4d17-94eb-35e517b76675.png)


Intelligence needs data. Data has to be collected, processed, and analyzed. Data collection is done from local sources such as network logs and public sources such as forums. Processing of data aims to arrange them into a format suitable for analysis. The analysis phase seeks to find more information about the attackers and their motives; moreover, it aims to create a list of recommendations and actionable steps.

Learning about your adversaries allows you to know their tactics, techniques, and procedures. As a result of threat intelligence, we identify the threat actor (adversary), predict their activity, and 
consequently, we will be able to mitigate their attacks and prepare a response strategy.

### Digital Forensics and Incident Response (DFIR)

This section is about Digital Forensics and Incident Response (DFIR), and we will cover:

- Digital Forensics
- Incident Response
- Malware Analysis

### Digital Forensics

Forensics is the application of science to investigate crimes and establish facts. With the use and spread of digital systems, such as computers and smartphones, a new branch of forensics was born to investigate related crimes: computer forensics, which later evolved into, *digital forensics*.

In defensive security, the focus of digital forensics shifts to analyzing evidence of an attack and its perpetrators and other areas such as intellectual property theft, cyber espionage, and possession of unauthorized content. Consequently, digital forensics will focus on different areas such as:

- **File System:** Analyzing a digital forensics image (low-level copy) of a system’s storage reveals much information, such as installed programs, created files, partially overwritten files, and deleted files.
- **System memory:** If the attacker is running their malicious program in memory without saving it to the disk, taking a forensic image (low-level copy) of the system memory is the best way to analyze its contents and learn about the attack.
- **System logs:** Each client and server computer maintains different log files about what is happening. Log files provide plenty of information about what happened on a system. Some traces will be left even if the attacker tries to clear their traces.
- **Network logs:** Logs of the network packets that have traversed a network would help answer more questions about whether an attack is occurring and what it entails.

### Incident Response

An *incident* usually refers to a data breach or cyber attack; however, in some cases, it can be something less critical, such as a misconfiguration, an intrusion attempt, or a policy violation. Examples of a cyber attack include an attacker making our network or systems inaccessible, defacing (changing) the public website, and data breach (stealing company data). How would you *respond* to a cyber attack? Incident response specifies the methodology that should be 
followed to handle such a case. The aim is to reduce damage and recover in the shortest time possible. Ideally, you would develop a plan ready for incident response.

The four major phases of the incident response process are:

1. **Preparation:** This requires a team trained and ready to handle incidents. Ideally, various measures are put in place to prevent incidents from happening in the first place.
2. **Detection and Analysis:** The team has the necessary resources to detect any incident; moreover, it is essential to further analyze any detected incident to learn about its severity.
3. **Containment, Eradication, and Recovery:** Once an incident is detected, it is crucial to stop it from affecting other systems, eliminate it, and recover the affected systems. For instance, when we notice that a system is infected with a computer virus, we would like to stop (contain) the virus from spreading to other systems, clean (eradicate) the virus, and ensure proper system recovery.
4. **Post-Incident Activity:** After successful recovery, a report is produced, and the learned lesson is shared to prevent similar future incidents.

![image](https://user-images.githubusercontent.com/66146701/202235564-ca6cabdf-f78b-4011-9d05-bef983e3bbd8.png)


### Malware Analysis

Malware stands for malicious software. *Software* refers to programs, documents, and files that you can save on a disk or send over the network. Malware includes many types, such as:

- Virus is a piece of code (part of a program) that attaches itself to a program. It is designed to spread from one computer to another; moreover, it works by altering, overwriting, and deleting files once it infects a computer. The result ranges from the computer becoming slow to unusable.
- Trojan Horse is a program that shows one desirable function but hides a malicious function underneath. For example, a victim might download a video player from a shady website that gives the attacker complete control over their system.
- Ransomware is a malicious program that encrypts the user’s files. Encryption makes the files unreadable without knowing the encryption password. The attacker offers the user the encryption password if the user is willing to pay a “ransom.”

![image](https://user-images.githubusercontent.com/66146701/202235638-1e6b2fdd-dd29-4167-971e-72aff1e7b769.png)


Malware analysis aims to learn about such malicious programs using various means:

1. Static analysis works by inspecting the malicious program without running it. Usually, this requires solid knowledge of assembly language (processor’s instruction set, i.e., computer’s fundamental instructions).
2. Dynamic analysis works by running the malware in a controlled environment and monitoring its activities. It lets you observe how the malware behaves when running.

![image](https://user-images.githubusercontent.com/66146701/202235698-d9450ea9-c15f-4b8a-84cf-8bb174115849.png)


### Practical Example of Defensive Security

![image](https://user-images.githubusercontent.com/66146701/202235742-b8e31718-297f-42ce-af16-e9bba50b32a5.png)


You are part of a *Security Operations Center* (SOC) responsible for protecting a bank. This bank’s SOC uses a *Security Information and Event Management* (SIEM) system. A SIEM gathers security-related information and events from various sources and presents them via one system. For instance, you would be notified if there is a failed login attempt or a login attempt from an unexpected geographic location. Moreover, with the advent of machine learning, a SIEM might detect unusual behavior, such as a user logging in at 3 AM when he usually logs in only during work hours.

In this exercise, we will interact with a SIEM to monitor the different events on our network and systems in real-time. Some of the events are typical and harmless; others might require further intervention from us. Find the event flagged in red, take note of it, and click on it for further inspection.

Next, we want to learn more about the suspicious activity or event. The suspicious event might have been triggered by an event, such as a local user, a local computer, or a remote IP address. To send and receive postal mail, you need a physical address; similarly, you need an IP address to send and receive data over the Internet. An IP address is a logical address that allows you to communicate over the Internet. We inspect the cause of the trigger to confirm whether the event is indeed malicious. If it is malicious, we need to take due action, such as reporting to someone else in the SOC and blocking the IP address.

![image](https://user-images.githubusercontent.com/66146701/202235823-594bc291-cad7-46e1-a7e1-2bdd3db186aa.png)
![image](https://user-images.githubusercontent.com/66146701/202235894-367e5c60-89a4-4c62-8bef-d6b891c746b1.png)
![image](https://user-images.githubusercontent.com/66146701/202235937-56fe576a-9aad-4d9f-84bd-b70a24b80f44.png)
![image](https://user-images.githubusercontent.com/66146701/202235964-511f65f3-6498-4aaa-87c7-ea05d089aff9.png)
![image](https://user-images.githubusercontent.com/66146701/202235998-5fa07022-5bd6-4b2e-82dd-0c8a797ae1e8.png)

![image](https://user-images.githubusercontent.com/66146701/202236034-20178ebb-c9f6-4bbd-8437-98f843cd4a4a.png)

## Careers in Cyber

### Security Analyst

![image](https://user-images.githubusercontent.com/66146701/202236139-7bab2b0f-65f3-438c-8287-682a4a71ba48.png)

`Responsible for maintaining the security of an organisation's data`

Security analysts are integral to constructing security measures across organisations to protect the company from attacks. Analysts explore and evaluate company networks to uncover actionable data and recommendations for engineers to develop preventative measures. This job role requires working with various stakeholders to gain an understanding of security requirements and the security landscape.

### Responsibilities

- Working with various stakeholders to analyze the cyber security throughout the company
- Compile ongoing reports about the safety of networks, documenting security issues and measures taken in response
- Develop security plans, incorporating research on new attack tools and trends, and measures needed across teams to maintain data security.

### Security Engineer

![image](https://user-images.githubusercontent.com/66146701/202236206-7ca49566-4b6d-4a72-b699-dba423d14c31.png)

`Design, monitor and maintain security controls, networks, and systems to help prevent cyberattacks`

Security engineers develop and implement security solutions using threats and vulnerability data - often sourced from members of the security workforce. Security engineers work across circumventing a breadth of attacks, including web application attacks, network threats, 
and evolving trends and tactics. The ultimate goal is to retain and adopt security measures to mitigate the risk of attack and data loss.

### Responsibilities

- Testing and screening security measures across software
- Monitor networks and reports to update systems and mitigate vulnerabilities
- Identify and implement systems needed for optimal security

### Incident Responder

![image](https://user-images.githubusercontent.com/66146701/202236268-934dd14f-9443-4961-955f-683eb75a313e.png)

`dentifies and mitigates attacks whilst an attackers operations are still unfolding`

Incident responders respond productively and efficiently to security breaches. Responsibilities include creating plans, policies, and protocols for organisations to enact during and following incidents. This is often a highly pressurised position with assessments and responses required in real-time, as attacks are unfolding. Incident response metrics include MTTD, MTTA, and MTTR - the meantime to detect, acknowledge, and recover (from attacks.) The aim is to achieve a swift 
and effective response, retain financial standing and avoid negative breach implications. Ultimately, incident responders protect the company's data, reputation, and financial standing from cyber attacks.

### Responsibilities

- Developing and adopting a thorough, actionable incident response plan
- Maintaining strong security best practices and supporting incident response measures
- Post-incident reporting and preparation for future attacks, considering learnings and adaptations to take from incidents

### Digital Forensics Examiner

![image](https://user-images.githubusercontent.com/66146701/202236352-c4c74a54-4d4e-4fcb-b7b6-698537aff23e.png)

`Responsible for using digital forensics to investigate incidents and crimes`

If you like to play detective, this might be the perfect job. If you are working as part of a law-enforcement department, you would be focused on collecting and analysing evidence to help solve crimes: charging the guilty and exonerating the innocent. On the other hand, if your work falls under defending a company's network, you will be using your forensic skills to analyse incidents, such as policy violations.

### Responsibilities

- Collect digital evidence while observing legal procedures
- Analyse digital evidence to find answers related to the case
- Document your findings and report on the case

### Malware Analyst

![image](https://user-images.githubusercontent.com/66146701/202236423-fe981841-af51-43bd-8dd8-aa628816044b.png)

`Analyses all types of malware to learn more about how they work and what they do`

A malware analyst's work involves analysing suspicious programs, discovering what they do and writing reports about their findings. A malware analyst is sometimes called a reverse-engineer as their core task revolves around converting compiled programs from machine language 
to readable code, usually in a low-level language. This work requires the malware analyst to have a strong programming background, especially in low-level languages such as assembly language and C language. The ultimate goal is to learn about all the activities that a malicious 
program carries out, find out how to detect it and report it.

### Responsibilities

- Carry out static analysis of malicious programs, which entails reverse-engineering
- Conduct dynamic analysis of malware samples by observing their activities in a controlled environment
- Document and report all the findings

### Penetration Tester

![image](https://user-images.githubusercontent.com/66146701/202236497-d963a31d-4f81-4583-9319-110985c4643c.png)

`Responsible for testing technology products for security loopholes`

You may see penetration testing referred to as pentesting and ethical hacking. A penetration tester's job role is to test the security of the systems and software within a company - this is achieved through attempts to uncover flaws and vulnerabilities through systemised 
hacking. Penetration testers exploit these vulnerabilities to evaluate the risk in each instance. The company can then take these insights to rectify issues to prevent a real-world cyberattack.

### Responsibilities

- Conduct tests on computer systems, networks, and web-based applications
- Perform security assessments, audits, and analyse policies
- Evaluate and report on insights, recommending actions for attack prevention

### Red Teamer

![image](https://user-images.githubusercontent.com/66146701/202236587-6be73f1e-7ee5-4966-9ce5-b951e6951164.png)

`Plays the role of an adversary, attacking an organisation and providing feedback from an enemies perspective`

Red teamers share similarities to penetration testers, with a more targeted job role. Penetration testers look to uncover many vulnerabilities across systems to keep cyber-defence in good standing, whilst red teamers are enacted to test the company's detection and response capabilities. This job role requires imitating cyber criminals' actions, emulating malicious attacks, retaining access, and avoiding detection. Red team assessments can run for up to a month, typically by a team external to the company. They are often best suited to organisations with mature security programs in place.

### Responsibilities

- Emulate the role of a threat actor to uncover exploitable vulnerabilities, maintain access and avoid detection
- Assess organisations' security controls, threat intelligence, and incident response procedures
- Evaluate and report on insights, with actionable data for companies to avoid real-world instances
