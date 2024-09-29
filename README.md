# 30 Days SOC Automation Challenge
 ELK Stack SOC automation using Fleet and OS Ticketing Server

## Day 1: Logical Diagram

🚀 Embarking on MYDFIR 30-Days SOC Challenge! by my mentor Steven ([link](https://lnkd.in/dRGfScbr)) 🚀  
I'm thrilled to announce that I'll be diving into an intensive Security Operations Center (SOC) simulation, where I'll be provisioning and managing a complex environment on VULTR Cloud. This project is designed to enhance my skills as a SOC Analyst by replicating real-world scenarios and challenges.

### Key Components of the Environment:
- 🖥️ **Windows Server with RDP enabled**: A critical asset in many infrastructures, ripe for security monitoring and attack vector simulation.
- 🎛️ **Fleet Server**: Centralizing management and monitoring of the environment, a key part of maintaining security posture.
- 🐧 **Ubuntu Server with SSH enabled**: Providing a platform to simulate and detect unauthorized access attempts.
- 📊 **ELK Stack Server**: A powerful tool for log aggregation, analysis, and visualization—essential for incident detection and response.
- 📋 **OS Ticketing Server**: Integrating with incident response processes to track and manage security incidents efficiently.
- 🎯 **Command and Control Server with Kali Linux**: The heart of the simulated attack, representing a persistent threat actor within the network.

What to Expect:  
Over the next 30 days, I’ll be sharing insights, challenges, and key learnings as I simulate attacks and respond to incidents in this environment. This journey promises to be both rigorous and rewarding, offering valuable lessons that I look forward to applying in real-world SOC operations.

Feel free to engage with your thoughts and questions along the way!

FREE $300 Cloud Credit (Vultr): [link](https://lnkd.in/drVeaA5s) - Only applies to new accounts.

---
![SOC LAB Image](https://github.com/Virus192/elk-soc-automation/blob/main/images/SOC%20LAB.jpg)



## [Day 2: ELK Stack Deep Dive](https://github.com/Virus192/Day-2-ELK-Stack-Deep-Dive)

🚀 **Day 2 of MYDFIR 30 Days SOC Challenge: We took a Deep Dive into the ELK Stack** 🚀  
Today we focus on the ELK Stack—a cornerstone technology in Security Operations Centers (SOC) for effective log management and threat analysis. 

### Technical Overview of the ELK Stack:
1. **Elasticsearch** 🗄️  
   **Function**: A highly scalable search and analytics engine.  
   **Role in SOC**: Stores and indexes vast amounts of log data, enabling quick search and real-time analysis of security events.

2. **Logstash** 🛠️  
   **Function**: A server-side data processing pipeline.  
   **Role in SOC**: Ingests data from various sources, transforms it, and sends it to Elasticsearch for indexing.

3. **Kibana** 📊  
   **Function**: A visualization and exploration tool.  
   **Role in SOC**: Provides interactive dashboards and visualizations of the data stored in Elasticsearch.

4. **Beats** 🐝  
   **Function**: Lightweight data shippers.  
   **Role in SOC**: Collects data from various sources and forwards it to Logstash or Elasticsearch for processing.

### Significance of ELK Stack in the SOC Project:
- **Centralized Log Management**: Aggregates logs from diverse sources into a single repository.
- **Real-Time Threat Detection**: Facilitates the swift identification of suspicious activities through real-time processing.
- **Scalability and Flexibility**: Handles large volumes of data, allowing the SOC to grow.
- **Customizable Dashboards**: Empowers SOC analysts to create tailored dashboards for critical security metrics.

---
![SOC LAB Image](https://raw.githubusercontent.com/Virus192/Day-2-ELK-Stack-Deep-Dive/main/images/1_EElZCCfA9S0kgABEDi5sOw.png)


## [Day 3: Building a Secure Elasticsearch Deployment](https://github.com/Virus192/Day-3-Building-a-Secure-Elasticsearch-Deployment)

🌟 **Day Three of #MYDFIRSOCChallenge: Building a Secure Elasticsearch Deployment** 🌟  
Special Thanks to MYDFIR for this exciting challenge!

Today was all about diving deep into the world of Elasticsearch Consulting! 🎯 As part of the #30DaysSOCChallenge, I had the opportunity to set up and secure an Elasticsearch instance, and it was an exciting ride. 🚀

### What's on the Plate?
- **Installed Elasticsearch on a robust Ubuntu 22.04 LTS environment**. 🐧
- **Ensured a secure deployment by implementing a well-configured firewall**. 🔒
- **Deployed within a VPC 2.0 on Vultr for enhanced network security**. 🌐

### Why Does This Matter?
Elasticsearch is a powerful tool in the SOC toolkit, enabling efficient search, analysis, and visualization of log data. However, ensuring its secure deployment is crucial to avoid becoming a target of the very threats we seek to defend against.

### Key Takeaways:
- **Ubuntu 22.04 LTS provides a stable and secure foundation for hosting Elasticsearch, minimizing vulnerabilities from the OS level.**
- **A secured firewall setup is non-negotiable—it keeps unwanted visitors at bay, protecting our data and services.**
- **Leveraging VPC 2.0 in Vultr adds an extra layer of network segmentation and security, isolating our deployment from potential threats.**

As I progress through this challenge, I'm constantly reminded of the importance of robust security practices in every layer of deployment. Looking forward to seeing how this setup will empower our security operations moving forward! 💪

FREE $300 Cloud Credit (Vultr): [Link](https://lnkd.in/drVeaA5s) - Only applies to new accounts.

![Elasticsearch Setup](https://raw.githubusercontent.com/Virus192/elk-soc-automation/main/images/photo_5960977688871158764_w.jpg)

## [Day 4: Elasticsearch Security Configuration](https://github.com/Virus192/Day-4-Elasticsearch-Security-Configuration)

---------------------------

### 🌟 It's Day 4 of the MYDFIR 30-Day SOC Automation Challenge.
 Here is our Task for today: Kibana Installation & Configuration 🌟
 Today's journey was all about setting up and configuring Kibana to visualize and analyze our Elasticsearch data. Here's how it all went down:

The generated password for the elastic built-in superuser is: `OK6A_2wP9DZql=hYsc1M`

If this node should join an existing cluster, you can reconfigure this with:
`/usr/share/elasticsearch/bin/elasticsearch-reconfigure-node --enrollment-token <token-here>`
after creating an enrollment token on your existing cluster.

You can complete the following actions at any time:

- Reset the password of the elastic built-in superuser with:
  `/usr/share/elasticsearch/bin/elasticsearch-reset-password -u elastic`.

- Generate an enrollment token for Kibana instances with:
  `/usr/share/elasticsearch/bin/elasticsearch-create-enrollment-token -s kibana`.

- Generate an enrollment token for Elasticsearch nodes with:
  `/usr/share/elasticsearch/bin/elasticsearch-create-enrollment-token -s node`.

### NOT starting on installation, please execute the following statements to configure Elasticsearch service to start automatically using systemd
```bash
sudo systemctl daemon-reload
sudo systemctl enable elasticsearch.service
```
![SOC](https://raw.githubusercontent.com/Virus192/elk-soc-automation/main/images/photo_5965442483469009319_w.jpg)

## [Day 5: Deploying a Windows Server on Vultr Cloud](https://github.com/Virus192/Day-5-Deploying-a-Windows-Server-on-Vultr-Cloud)

🌟 **Day 5 of MYDFIR 30 Days SOC Challenge: Deploying a Windows Server on Vultr Cloud** 🌟

Today, I deployed a Windows Server on Vultr Cloud, moving it out of VPC 2.0 for public accessibility.

## Quick Steps

1. **Login to Vultr Cloud** and click on the **Deploy +** button.
2. **Choose Server Type:** Cloud Compute — Shared CPU.
3. **Select Plan:** 55GB SSD, 1 vCPU, 2GB memory.
4. **Deploy:** Click **Deploy Now** and wait 5-7 minutes.
5. **Access:** Use the provided credentials to log in.

Deploying a Windows Server on Vultr Cloud is a simple process, ideal for making your server publicly accessible while keeping costs low.


![Windows Server Deployment](https://raw.githubusercontent.com/Virus192/elk-soc-automation/main/images/1_VCKRGZAd1IWFjfHcdCKCDg.png)

## [Day 6: Introduction to Fleet Server and Elastic Agent](https://github.com/Virus192/Day-6-Introduction-to-Fleet-Server-and-Elastic-Agent)

 🌟 **Day 6 of MYDFIR 30 Days SOC Challenge: Exploring Fleet Server and Elastic Agent** 🌟

Today’s focus is on mastering the centralized management of Elastic Agents using Fleet Server, an essential tool for large-scale environments.

Imagine deploying Elastic Agents on 100 Windows machines to monitor PowerShell logs, only to realize they’re not forwarding logs to your Elasticsearch instance. What would you do? Instead of manually reconfiguring each endpoint, you could use Fleet Server to handle everything centrally.

## Key Components

### Elastic Agent

- A unified tool for monitoring logs, metrics, and other data types, with policies you can update remotely.
- Two modes of installation:
  - **Fleet Managed Mode:** Centralized management
  - **Standalone:** Manual setup

### Fleet Server

- The backbone of centralized agent management, allowing you to:
  - Deploy policies
  - Add integrations
  - Update agents across all endpoints with ease

## Why Use Fleet Server?

- **Centralized Management:** Control agent policies and integrations from one dashboard.
- **Seamless Updates:** Easily push updates to all agents at once, saving hours of manual work.
- **Simplified Unenrollment:** Unenroll agents with just a few clicks, eliminating the need to touch every machine.

Leveraging Fleet Server simplifies your SOC operations, ensuring efficient data collection and security monitoring across your environment.

![insert image here](image.jpg)


## [Day 7: Setting Up Elastic Fleet Server and Enrolling Windows Server](https://github.com/Virus192/Day-7-Setting-Up-Elastic-Fleet-Server-and-Enrolling-Windows-Server)

🌟 **Day 7 of MYDFIR 30 Days SOC Challenge: Setting Up Elastic Fleet Server and Enrolling a Windows Server Using Elastic Agent** 🌟

Today's challenge dives into centralizing the management and monitoring of multiple servers using Elastic Fleet and Elastic Agent. We set up a Fleet Server on Vultr, installed an Elastic Agent on a Windows Server, and enrolled it into our fleet for seamless monitoring.

## Steps to Achieve This:

### 1. Create Fleet Server on Vultr

- Deployed a Fleet Server using Ubuntu 22.04 LTS on Vultr.
- Selected **Optimized Cloud Compute** for enhanced performance and security.

### 2. Configure Fleet in Elastic

- Accessed Elastic's GUI, navigated to the **Fleet Management** tab, and added a new Fleet Server.
- Generated the **Fleet Service Policy** and **Service Token** required for connecting the Elastic Agent.

### 3. Install Elastic Agent on Fleet Server

- SSH'd into the Fleet Server, updated the system, and installed the Elastic Agent using the Elastic GUI-generated command.
- Configured firewall rules to allow necessary traffic on ports 9200 and 8200.

### 4. Enroll Windows Server

- Installed the Elastic Agent on a Windows Server via PowerShell.
- The Windows Server was successfully enrolled and connected to the Fleet for centralized monitoring.

## Outcome

Successfully deployed a Fleet Server and enrolled a Windows Server, enabling real-time monitoring of logs and metrics through the Elastic Stack. This setup enhances our SOC’s ability to maintain operational visibility and detect potential threats.

![insert image here](image.jpg)


## [Day 8: Installing Sysmon on a Windows Server](https://github.com/Virus192/Day-8-Installing-Sysmon-on-a-Windows-Server)


**Day 8 of MYDFIR 30 Days SOC Challenge: Installing Sysmon for Advanced Telemetry** 🚀

Today’s focus was on enhancing our visibility into system activity by installing Sysmon (System Monitor) on a Windows Server. Sysmon is a critical tool for SOC environments, providing detailed telemetry that aids in detecting suspicious activities and bolstering security.

## Step-by-Step Highlights

1. **Download Sysmon and Configuration File**
   - Downloaded Sysmon and the popular Sysmon Olaf Configuration file from GitHub, which guides what system events to log.

2. **Install Sysmon**
   - Installed Sysmon using PowerShell and configured it with the downloaded configuration file.

3. **Verify Telemetry**
   - Verified telemetry by checking the Sysmon logs in the Event Viewer, ensuring it captures key activities such as process creation and network connections.

Sysmon is now actively monitoring the Windows Server, providing valuable insights into system events. Another day, another tool deployed in our SOC environment—helping us stay one step ahead of potential threats. 💻🔒

Stay tuned for more security setups!

![insert image here](image.jpg)

## [Day 9: Introduction to Sysmon](https://github.com/Virus192/Day-9-Introduction-to-Sysmon)

 🌟 **Day 9 of MYDFIR 30 Days SOC Challenge: Introduction to Sysmon** 🌟

Today's focus was all about enhancing endpoint visibility with Sysmon—a crucial tool for security analysts in detecting and responding to advanced threats. In the world of cybersecurity, having detailed logs of system activities is essential, and Sysmon steps in to provide that extra layer of monitoring.

## 🔍 What is Sysmon?

Sysmon, part of Microsoft's Sysinternals Suite, is a tool that logs critical system events like process creation, network connections, and file modifications. It goes beyond default Windows logging by offering highly detailed telemetry that allows SOC analysts to track malicious activity in real time. Using a customizable configuration file, Sysmon can fine-tune the events you want to monitor, making it an invaluable asset during investigations.

## 💡 Key Capabilities

- **Process Creation Logging**: Tracks newly created processes with detailed command-line information.
- **File Hashing**: Logs file hashes (SHA1, MD5, etc.) to aid in threat intelligence and OSINT.
- **Network Connection Monitoring**: Records inbound/outbound connections, crucial for detecting C2 activities.
- **Dynamic Rule Filtering**: Focus on the most relevant events by customizing rule-based filters.

Sysmon empowers SOC teams to gain deeper insights into endpoint activities, offering the ability to detect attacks early and correlate events across different logs using unique Process GUIDs.

Stay tuned for more insights tomorrow as we dive deeper into endpoint monitoring with Sysmon! 💪

![insert image here](image.jpg)

## [Day 10: Ingesting Sysmon and Windows Defender Logs into Elasticsearch](https://github.com/Virus192/Day-10-Ingesting-Sysmon-and-Windows-Defender-Logs-into-Elasticsearch)


🚀 **Day 10 of MYDFIR 30 Days SOC Challenge: Ingesting Sysmon and Windows Defender Logs into Elasticsearch** 🚀

Today’s focus was on enhancing visibility into our Windows environment by setting up log ingestion for Sysmon and Windows Defender into Elasticsearch. This process allows for powerful log analysis and real-time threat detection within the SOC.

#### Key Steps:

🛠️ **Elastic Integrations**: Configured Sysmon and Windows Defender logs using Elastic’s GUI. For each integration:
- Named and described the log sources, using Event Viewer to locate the correct channels.
- Specified event IDs for Windows Defender to capture critical security actions, such as detecting malware and real-time protection status.

🔒 **Firewall Configuration**: Ensured logs could be transmitted to Elasticsearch by setting up firewall rules to allow TCP traffic on port 9200.

🔍 **Log Verification**: Used Elastic’s Discover feature to verify that the logs were being ingested properly, focusing on key event IDs (like `winlog.event_id: 5001` for Windows Defender).

With Sysmon and Windows Defender logs now integrated, we’ve built a solid foundation for monitoring and responding to security events within our Windows infrastructure.

![insert image here](image.jpg)

## [Day 11: Fortify Your Digital Walls with Brute Force Attack Prevention](https://github.com/Virus192/Day-11-Fortify-Your-Digital-Walls-with-Brute-Force-Attack-Prevention)

🔐 **Day 11 of MYDFIR 30 Days SOC Challenge: Fortify Your Digital Walls with Brute Force Attack Prevention** 🔐

Today’s insight centers around **Brute Force Attacks** — the digital equivalent of trying every key in the world to unlock your door. Hackers use this method to guess passwords and gain unauthorized access to accounts and systems.

### Types of Brute Force Attacks 🔍
1. **Simple Brute Force**: Trying all possible character combinations.
2. **Dictionary Attack**: Using a list of common words or passwords.
3. **Credential Stuffing**: Reusing passwords leaked from data breaches.

### How to Defend Yourself ⚔️
1. **Strong, Unique Passwords**: Use long, complex passwords or passphrases.
2. **Multi-Factor Authentication (MFA)**: Add a second layer of security.
3. **Password Manager**: Safely store and manage unique passwords.
4. **Stay Vigilant**: Watch out for phishing attempts.
5. **Regular Updates**: Change passwords regularly, especially after breaches.

### Common Brute Force Tools 💻
While tools like **Hydra**, **Hashcat**, and **John the Ripper** exist, they should only be used ethically, with permission, for security testing.

Brute force attacks are persistent but preventable. Stay informed, protect your data, and keep the hackers out! 🌐✨

