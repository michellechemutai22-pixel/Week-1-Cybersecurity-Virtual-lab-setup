# Week-1-Cybersecurity-Virtual-lab-setup
Penetration Testing Virtual Lab – Kali Linux

<ins>##Project Overview</ins>
The project was about setting up a virtual lab using virtualBox and kali-linux.
The purpose of the lab is to create a safe environment to  Use specialized security distributions (like Kali Linux) and practice penetration testing or vulnerability exploitation on intentionally vulnerable targets and also  Run malware, test aggressive cyberattacks, or configure volatile system settings in a sandboxed space where crashes or infections cannot harm the main computer.

<ins>##Purpose of the lab</ins>
The primary purpose of creating a virtual penetration-testing environment is to provide a completely isolated, legal, and safe sandbox to practice offensive security tactics without risking damage to production networks or breaking the law.
A sandbox is important because it acts as an isolated digital quarantine, allowing you to run untrusted code, execute malware, or test volatile system changes without any risk to your host computer, network, or data.
The network in a virtual penetration-testing environment must be isolated to prevent active exploits, malicious payloads, and automated network traffic from escaping into your home network or the public internet.
Virtualization isolates the hardware and software layers, creating an entirely self-contained environment where actions taken inside a virtual machine have no physical or operational impact on your actual computer or network. It accomplishes this through a specialized software layer called a hypervisor, which acts as a strict referee between your physical computer (the host) and your practice environments.

<ins>##Lab Environment</ins>
### Lab Environment

| Component                       | Details           |
| ------------------------------- | ----------------- |
| **Host Operating System**       | Windows 11        |
| **Virtualization Software**     | Oracle VirtualBox |
| **Kali Linux Version**          | Kali Linux 2026.2 |<img width="908" height="393" alt="Virtualbox NAT networks configuration" src="https://github.com/user-attachments/assets/dffcc1a6-f828-45f8-8a31-9c73d52d5fb8" />

| **Host RAM**                    | 8 GB              |
| **RAM Allocated to Kali Linux** | 1.92 GB           |
| **CPU Usage**                   | 9%                |
| **Network Type**                | NAT Network       |
| **Network Address**             | 10.0.0.0/24       |
| **Kali Linux IP Address**       | 10.0.0.3/24       |

<ins>##Step-by-Step Lab Build</ins>
Step 1: Install 7-Zip
I installed 7-Zip on the Windows 11 host machine to extract the compressed Kali Linux virtual machine files.

Step 2: Install Oracle VirtualBox
I installed Oracle VirtualBox on the Windows 11 host machine as a hypervisor.

Step 3: Create the NAT Network
I created a NAT Network in Oracle VirtualBox and configured it to use the network address 10.0.0.0/24.
<img width="908" height="393" alt="Virtualbox NAT networks configuration" src="https://github.com/user-attachments/assets/3bea8f72-fa8b-447c-8cb8-c4841b776b47" />
The NAT Network allows the virtual machines in the penetration-testing lab to communicate with each other while also providing access to external networks when required. Using a dedicated virtual network helps keep the lab environment separate from the host machine's normal network.

Step 4: Import Kali Linux into VirtualBox
I imported the extracted Kali Linux virtual machine into Oracle VirtualBox.
Importing the preconfigured Kali Linux virtual machine makes it possible to run Kali in an isolated virtual environment for penetration-testing practice.
<img width="1920" height="891" alt="VirtualBox_kali-linux-2026 2-virtualbox-amd64_14_08_2026_20_25_28" src="https://github.com/user-attachments/assets/1cda89c1-d0ac-4056-b176-d6aaa7e67283" />

Step 5: Configure the Kali-linux Network
You must configure the network settings inside Kali Linux to match your VirtualBox settings because the virtual network adapter inside Kali must align with the virtual switch VirtualBox creates in your RAM. 
<img width="587" height="401" alt="Kali linux configuration to NAT networks" src="https://github.com/user-attachments/assets/ea693620-fdc4-44ff-8592-670ec8433198" />.

Step 6: Running a command in kali-linux 2026-2 terminal
<img width="1920" height="891" alt="Running a command in kali linux 2026 2" src="https://github.com/user-attachments/assets/bf7dd9d0-9b72-4158-894a-2721cd62bdec" />

Step 7: Checking network connection
<img width="1920" height="891" alt="Checking network connection in the kali linux terminal" src="https://github.com/user-attachments/assets/26890593-b3ed-4652-ab7c-1c0c8e37a088" />

Step 8: Verifying internet connection 
<img width="1920" height="891" alt="Verifying internet connection in Kali linux terminal" src="https://github.com/user-attachments/assets/b0a3afda-5b7d-42c2-9e27-08d960f87f3f" />

<ins>##Snapshot</ins>
Snapshots act like a digital "Undo" button or a save-point in a video game. They freeze the exact state of a virtual machine—including its virtual hard disk, settings, and optionally its active RAM—at a precise moment.
Snapshots protect you from logical failures, software instability, and lab contamination.
<img width="528" height="176" alt="snapshot screenshot" src="https://github.com/user-attachments/assets/1fc32835-94bc-49dd-a762-96799c29e74e" />

<ins>##What I Learned This Week</ins>
 when running a penetration testing or malware analysis lab—is that a snapshot is NOT a backup, and relying on it as one can lead to total data loss.
 Kali-linux innstallation
 Network configuration in a virtualBox and kali-linux.
 How to take a snapshot.

 <ins>##Tools and Resources</ins>
 Oracle VirtualBox
Kali Linux 2026.2
Windows
ip addr
ping

<ins>##Author</ins>
Michelle Chemutai
Cybersecurity Professional B082
LinkedIn: www.linkedin.com/in/michellechemutai













