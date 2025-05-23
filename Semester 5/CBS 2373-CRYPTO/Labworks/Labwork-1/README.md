# Lab 1: Cryptographic Attacks: Brute Force and Traffic Analysis on Network Protocols

## 🔐 **Objective**
In this lab, you will explore the security weaknesses of commonly used network protocols (FTP, TELNET, SSH, and HTTP). The primary focus will be on performing **brute force attacks** to recover passwords and **network traffic sniffing** to analyze data transmission. You will also enhance your understanding of how to secure these protocols by identifying vulnerabilities and suggesting mitigation strategies.

---

## 🛠️ **What You’ll Need**

| Tools              | Purpose                  |
|--------------------|--------------------------|
| Metasploitable 2    | Practice attacks         |
| Kali Linux         | Attacker Machine         |
| Hydra              | Brute force tool         |
| Medusa             | Brute force tool         |
| NetExec            | Brute force tool         |
| Burp Intruder      | HTTP login automation    |
| Wireshark          | Network traffic analysis |

---

## 📝 **Lab Tasks**

### 1. 🔍 **Discover Usernames for Brute Force Attacks** 
- **Goal**: Explore the vulnerable VM to **enumerate potential usernames**.
- **Action**: Identify usernames to target with brute force and document your findings for later use.

### 2. ⚔️ **Launch Brute Force Attacks** 
#### 2.1. 💻 **FTP, TELNET, and SSH**
- **Tools**: Use **Hydra**, **Medusa**, or **NetExec** to perform brute force attacks on FTP, TELNET, and SSH.
  - **FTP**: Gain unauthorized access to the FTP service.
  - **TELNET**: Crack the password and access the TELNET service.
  - **SSH**: Use the same brute force techniques to gain access to SSH.

#### 2.2. 🌐 **HTTP Login Page** 
- **Tool**: Use **Burp Intruder** to automate attacks against an **HTTP login page**.
  - **Configure**: Set Intruder to test a list of usernames and passwords.
  - **Analyze**: Check for any successful logins and document your results.

### 3. 🕵️‍♂️ **Sniff Network Traffic** 
- Once you’ve cracked the credentials, **log in** to the services and start **sniffing network traffic**.
- **Tools**: Use **Wireshark** or **tcpdump** to capture and analyze network traffic.
- **Objective**: Look for **plaintext** data (which is insecure) and **encrypted** data (which is secure).
- **Deliverables**: Provide screenshots and analysis of which protocols are vulnerable and which are secure.

### 4. 🛠️ **Troubleshoot and Problem Solve** 
- **Questions to Consider**:
  - Did you encounter any challenges while performing brute force attacks (e.g., **rate limiting** or protocol-specific issues)?
  - **How did you solve these challenges**? Share your troubleshooting methods and solutions.

### 5. 🔒 **Suggest Mitigation Strategies** 
- For each protocol tested, propose **secure alternatives** to avoid the vulnerabilities discovered.
  - **Explain** how these alternatives can improve security and protect against brute force and traffic sniffing.

---

## 🎯 **Final Notes**
- This lab will give you hands-on experience in **attacking and securing** network protocols, teaching you both offensive and defensive cryptographic techniques.
- Be sure to document all your findings and challenges along the way. This will not only help you in understanding vulnerabilities but also in implementing secure solutions.
