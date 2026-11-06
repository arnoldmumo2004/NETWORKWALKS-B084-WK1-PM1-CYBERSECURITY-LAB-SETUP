# 🔐 Cybersecurity Lab Environment Setup

### Building an isolated virtual lab for penetration testing and ethical hacking practice

![Lab Architecture](screenshots/title%20image.png)

---

# 📌 Project Overview

This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using Oracle VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.

The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

---

# 🎯 Objectives

The main objectives of this project are to:

- Install and configure Oracle VirtualBox.
- Import Kali Linux as a virtual machine.
- Create a private NAT Network for the cybersecurity lab.
- Configure network connectivity for Kali Linux.
- Assign a consistent IP address to the Kali VM.
- Verify network connectivity and DNS resolution.
- Enable shared clipboard and drag-and-drop functionality.
- Configure shared folders.
- Take a clean VM snapshot for recovery.
- Document the complete setup process.
- Prepare the environment for future cybersecurity projects.

---

# 🛡️ Purpose of the Lab

The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.

### It can be used for activities such as:

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
- Linux administration
- Security tool experimentation
- Ethical hacking practice

⚠️ Important: This laboratory must only be used for systems that you own or have explicit permission to test.

---

# 🏗️ Lab Architecture

```text
Host Operating System (Windows 11)
          │
          │
    Oracle VirtualBox
          │
          │
      NatNetwork
     10.0.0.0/24
          │
          │
    Kali Linux VM
      10.0.0.2/24
```

---

# ⚙️ Lab Configuration

| Component | Configuration |
|------------|--------------|
| Host OS | Windows 11 |
| Hypervisor | Oracle VirtualBox |
| Security OS | Kali Linux 2026.3 |
| Virtual Network | NAT Network |
| Network Address | 10.0.0.0/24 |
| Kali IP Address | 10.0.0.2/24 |
| Gateway | 10.0.0.1 |
| Shared Clipboard | Bidirectional |
| Drag & Drop | Bidirectional |
| Shared Folder | Downloads Folder |
| Snapshot | Week1_Fresh_Kali_Lab |

---

# 🧪 Lab Setup Procedure

## Step 1: Install Oracle VirtualBox

Oracle VirtualBox was installed successfully and configured as the virtualization platform used throughout this project.

---

## Step 2: Create NAT Network

A dedicated NAT Network was created in VirtualBox.

Configuration:

```text
Network Name: NatNetwork
IPv4 Prefix: 10.0.0.0/24
DHCP: Enabled
```

### Screenshot

![NAT Network](screenshots/Network%20settings.jpeg)

---

## Step 3: Import Kali Linux

The official Kali Linux VirtualBox image was downloaded and imported successfully into Oracle VirtualBox.

### Screenshot

![Kali Linux](screenshots/Kali%20Linux%20Image.jpeg)

---

## Step 4: Configure the Kali Linux Network

The Kali Linux network settings were configured manually with a static IP address.

Configuration:

```text
IP Address: 10.0.0.2
Subnet Mask: /24
Gateway: 10.0.0.1
```

### Screenshot

![Kali Network Settings](screenshots/Kali%20Linux%20Network%20settings.jpeg)

---

## Step 5: Enable Shared Resources

The following VirtualBox features were enabled:

- Shared Clipboard (Bidirectional)
- Drag and Drop (Bidirectional)
- Shared Folder (Downloads Folder)

These settings allow smooth interaction between the Windows host machine and the Kali Linux virtual machine.

---

## Step 6: Verify Internet Connectivity

Internet connectivity was successfully verified.

Verification included:

- Accessing websites
- DNS resolution
- Network communication

✅ Internet connectivity successfully verified.

---

## Step 7: Create Snapshot

A recovery snapshot was created after completing all configurations.

Snapshot Name:

```text
Week1_Fresh_Kali_Lab
```

This snapshot serves as a clean recovery point for future cybersecurity labs.

---

# 🔍 Lab Verification

| Test | Result |
|--------|---------|
| VirtualBox Installed | ✅ PASS |
| NAT Network Created | ✅ PASS |
| Kali Linux Imported | ✅ PASS |
| Static IP Configured | ✅ PASS |
| Internet Connectivity Verified | ✅ PASS |
| Shared Clipboard Enabled | ✅ PASS |
| Drag and Drop Enabled | ✅ PASS |
| Shared Folder Configured | ✅ PASS |
| Snapshot Created | ✅ PASS |

-:

- Virtualization Technology
- Oracle VirtualBox Administration
- Kali Linux Setup and Configuration
- Virtual Networking
- NAT Network Configuration
- Linux Networking
- IP Addressing
- Cybersecurity Lab Design
- VM Snapshot Management
- Troubleshooting Virtual Environments

---

# 🚧 Challenges Encountered

## Challenge

Initial Kali Linux installation using an ISO image failed during the software installation process.

## Solution

The issue was resolved by using the official Kali Linux VirtualBox image, which provided a pre-configured and stable environment for the lab setup.

---

# 🎓 Conclusion

The cybersecurity laboratory environment was successfully created using Oracle VirtualBox and Kali Linux.

The environment is now ready for future cybersecurity projects, penetration-testing exercises, vulnerability assessments, and ethical hacking activities as part of the NetworkWalks Cybersecurity Internship Program.

---

# 👨‍💻 Author

**Arnold Mumo Kilonzo**

Bachelor of Science in Information Technology  
University of Embu

**Career Interests**
- Cybersecurity
- Network Administration & Management
- IT Support
- Generative AI
- Prompt Engineering
