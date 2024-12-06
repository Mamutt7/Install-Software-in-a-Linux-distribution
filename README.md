# Install Software in a Linux Distribution

This hands-on project demonstrates the basics of managing software installations, uninstallations, and verifications using the APT package manager in a Linux environment. Each task includes step-by-step instructions, commands, expected outputs, and screenshots to enhance understanding.

# Task 1: Ensure APT is Installed

Step 1: Open the terminal and check if the APT package manager is installed:
apt --version

Expected Output:
apt 1.8.2.3 (amd64)
Usage: apt [options] command
...

Screenshot:
![APT Installed](https://github.com/user-attachments/assets/9fc99d2f-bec4-428d-854d-9de33fcfcc33)

# Task 2: Install and Uninstall the Suricata Application

Step 1: Install Suricata:
sudo apt install suricata

Step 2: Verify Installation:
suricata --version

Expected Output:
Suricata 4.1.2
USAGE: suricata [OPTIONS] [BPF FILTER]
   -c   : path to configuration file
   -T   : test configuration file (use with -c)

Screenshot:
![Suricata Installed](https://github.com/user-attachments/assets/9bda91a2-530c-42d3-bb34-8e305e8b9559)

Step 3: Uninstall Suricata:
sudo apt remove suricata

Step 4: Verify Uninstallation:
suricata

Expected Output:
-bash: /usr/bin/suricata: No such file or directory

Screenshot:
![Suricata Uninstalled](https://github.com/user-attachments/assets/5ab18ee5-8888-4c23-9f13-c58aefe0d5e8)

# Task 3: Install the tcpdump Application

Step 1: Install tcpdump:
sudo apt install tcpdump

Screenshot:
![tcpdump Installed](https://github.com/user-attachments/assets/04729525-b476-4f00-9264-9630bd5a2206)

# Task 4: List Installed Applications

Step 1: List all installed applications:
apt list --installed

Step 2: Search for a specific application (e.g., tcpdump):
apt list --installed | grep tcpdump

Expected Output:
tcpdump/oldstable,now 4.9.3-1~deb10u2 amd64 [installed]

Screenshot:
![List Installed Applications](https://github.com/user-attachments/assets/e722ae0d-fc85-4b74-850b-546d5ed13862)

# Task 5: Reinstall the Suricata Application

Step 1: Reinstall Suricata:
sudo apt install suricata

Step 2: Verify Installation:
apt list --installed | grep suricata

Expected Output:
suricata/oldstable,now 1:4.1.2-2+deb10u1 amd64 [installed]
tcpdump/oldstable,now 4.9.3-1~deb10u2 amd64 [installed]

Screenshot:
![Suricata Reinstalled](https://github.com/user-attachments/assets/28818250-f4c7-4531-8132-665e05387b81)

# Conclusion

In this project, you learned the following:
- Installed Applications: Used the APT package manager to install applications.
- Uninstalled Applications: Removed applications and verified their absence.
- Verified Installed Applications: Checked for the presence of installed applications and their versions.

This hands-on experience is foundational for roles in cybersecurity, system administration, and cloud computing.
