🛡️ HYDRA-BASED BRUTE FORCE ATTACK DEMONSTRATION

📌 INTRODUCTION

This project demonstrates an FTP Brute Force Attack using Hydra in a controlled and isolated lab environment.

The practical is performed using Kali Linux as the attacking machine and Metasploitable 2 as the target machine.

The main purpose of this project is to understand how brute force attacks work, how Hydra is used for password testing, and why strong password security is important.

---

🛠️ TOOLS AND TECHNOLOGIES USED

- Kali Linux – Attacking Machine
- Hydra – Brute Force Testing Tool
- Nmap – Network Scanning and Service Detection
- Metasploitable 2 – Vulnerable Target Machine
- FTP – File Transfer Protocol
- VMware – Virtualization Platform

---

🎯 PROJECT OBJECTIVES

- Understand the concept of Brute Force Attacks.
- Learn how to use the Hydra tool.
- Identify FTP services using Nmap.
- Perform FTP authentication security testing.
- Understand weak password vulnerabilities.
- Learn the importance of strong password security.

---

🧪 LAB ENVIRONMENT

Component| Details
Attacker Machine| Kali Linux
Target Machine| Metasploitable 2
Testing Tool| Hydra
Scanning Tool| Nmap
Target Service| FTP
Default FTP Port| 21
Virtualization| VMware

---

📸 PRACTICAL IMPLEMENTATION AND SCREENSHOTS

01. METASPLOITABLE IP ADDRESS

"Metasploitable IP" (./01_Metasploitable_IP.PNG)

Command Used:

ifconfig

Description:

Identified the IP address of the Metasploitable 2 target machine for lab testing.

---

02. KALI LINUX DESKTOP

"Kali Desktop" (./02_Kali_Desktop.jpg)

Description:

Started the Kali Linux virtual machine and prepared the environment for security testing.

---

03. HYDRA INSTALLATION

"Hydra Installation" (./03_Hydra_Installation.PNG)

Command Used:

sudo apt install hydra

Description:

Installed Hydra, a password security testing tool used for authentication testing.

---

04. NMAP SERVICE DETECTION

"Nmap Service Detection" (./04_Nmap_Service_Detection.PNG)

Command Used:

nmap -sV -p 21 <TARGET-IP>

Description:

Scanned the target machine to identify the FTP service and detect its version.

---

05. PASSWORD FILE

"Password File" (./05_Swayapass_File.PNG)

Command Used:

cat password.txt

Description:

Prepared a password list for controlled authentication security testing.

---

06. PASSWORD FILE VERIFICATION

"Password File Verification" (./06_Password_File_Verification.PNG)

Command Used:

ls -l

Description:

Verified the password file and checked its availability in the working directory.

---

07. FTP SERVICE RESULT

"FTP Service Result" (./07_FTP_Service_Result.PNG)

Command Used:

ftp <TARGET-IP>

Description:

Connected to the target FTP service and examined its authentication process.

---

08. HYDRA FINAL TESTING

"Hydra Final Testing" (./09_Hydra_Final_Testing.PNG)

Command Used:

hydra -l <USERNAME> -P password.txt ftp://<TARGET-IP>

Description:

Performed authorized FTP password testing using Hydra against the isolated Metasploitable 2 lab machine.

---

09. FTP FINAL CONNECTION

"FTP Final Connection" (./10_FTP_IP_Connection.PNG)

Command Used:

ftp <TARGET-IP>

Description:

Verified FTP connectivity with the target machine after completing the security testing.

---

🔐 SECURITY RECOMMENDATIONS

- Use Strong Passwords: Create long and complex passwords.
- Enable Multi-Factor Authentication: Add an extra layer of account security.
- Implement Login Rate Limiting: Restrict repeated login attempts.
- Monitor Failed Login Attempts: Regularly check authentication logs.
- Disable Unused Services: Reduce unnecessary network exposure.
- Use Secure Protocols: Prefer SFTP instead of FTP.

---

📚 LEARNING OUTCOMES

Through this project, I learned:

- Basic concepts of Brute Force Attacks.
- Installation and usage of Hydra.
- Network scanning using Nmap.
- FTP service identification and testing.
- Password security and authentication risks.
- Basic security measures against brute force attacks.

---

⚠️ DISCLAIMER

This project is created strictly for educational and cybersecurity learning purposes.

All testing was performed in an isolated lab environment using Metasploitable 2.

Unauthorized access or testing against systems without permission is strictly prohibited.

---

👨‍💻 AUTHOR

Swayam Gite

Cyber Security Enthusiast | Aspiring SOC Analyst
