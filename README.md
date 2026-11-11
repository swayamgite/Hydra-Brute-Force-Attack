🛡️ HYDRA-BASED BRUTE FORCE ATTACK DEMONSTRATION

📌 INTRODUCTION

This project demonstrates FTP authentication security testing using Hydra in a controlled and isolated lab environment.

The practical is performed using Kali Linux as the attacking machine and Metasploitable 2 as the target machine.

The main objective is to understand brute force attacks, identify FTP services, perform password security testing, and learn security protection techniques.

🛠️ TOOLS USED

- Kali Linux
- Hydra
- Nmap
- Metasploitable 2
- FTP
- VMware

🎯 PROJECT OBJECTIVES

- Understand Brute Force Attack concepts.
- Learn Hydra tool usage.
- Identify FTP services using Nmap.
- Perform FTP authentication testing.
- Understand weak password security.
- Learn preventive security measures.

🧪 LAB ENVIRONMENT

Component| Details
Attacker Machine| Kali Linux
Target Machine| Metasploitable 2
Target Service| FTP
Port Number| 21
Testing Tool| Hydra
Scanning Tool| Nmap
Platform| VMware

---

📸 PRACTICAL IMPLEMENTATION

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

"Password File" (./05_Samypass_File.PNG)

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

Performed authorized FTP password testing against the isolated Metasploitable 2 lab machine using Hydra.

---

09. FTP FINAL CONNECTION

"FTP Final Connection" (./10_FTP_IP_Connection.PNG)

Command Used:

ftp <TARGET-IP>

Description:

Verified FTP connectivity with the target machine after completing the security testing.

---

🔐 SECURITY RECOMMENDATIONS

- Strong Passwords: Use long and complex passwords.
- Multi-Factor Authentication: Enable an additional authentication layer.
- Login Rate Limiting: Restrict repeated login attempts.
- Log Monitoring: Monitor failed login attempts.
- Secure Protocols: Prefer SFTP instead of FTP.
- Disable Unused Services: Reduce unnecessary network exposure.

---

📚 LEARNING OUTCOMES

Through this project, I learned:

- Brute Force Attack concepts.
- Hydra installation and usage.
- Nmap network scanning.
- FTP service detection and testing.
- Password security risks.
- Basic security protection techniques.

---

⚠️ DISCLAIMER

This project is created strictly for educational and cybersecurity learning purposes.

All testing was performed in an isolated lab environment using Metasploitable 2.

Unauthorized access or testing against systems without permission is strictly prohibited.

---

👨‍💻 AUTHOR

Swayam Gite

Cyber Security Enthusiast | Aspiring SOC Analyst                                 
