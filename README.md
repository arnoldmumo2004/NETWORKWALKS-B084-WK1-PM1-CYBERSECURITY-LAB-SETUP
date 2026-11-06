# 🔐 Cybersecurity Lab Environment Setup

### Building an isolated virtual lab for penetration testing and ethical hacking practice

![Kali Linux Environment](Kali%20Linux%20Image.jpeg)

---

# 📌 Project Overview

This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using Oracle VirtualBox and Kali Linux.

The purpose of this lab is to create a controlled environment where cybersecurity tools, network scanning, vulnerability assessment, reconnaissance, and other security-testing activities can be performed safely and repeatedly.

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
- Configure shared folders between the host and virtual machine.
- Take a clean VM snapshot for recovery.
- Document the complete setup process.
- Prepare the environment for future cybersecurity projects.

---

# 🛡️ Purpose of the Lab

The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.

It can be used for activities such as:

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
- Exploitation practice
- Security-tool experimentation
- Linux administration

⚠️ **Important:** This laboratory must only be used for systems that you own or have explicit permission to test.

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
      10.0.0.2
```

Additional target machines can be added later for cybersecurity practice and penetration testing exercises.

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
| Drag and Drop | Bidirectional |
| Shared Folder | Downloads Folder |
| Snapshot | Week1_Fresh_Kali_Lab |

---

# 🧪 Lab Setup Procedure

## Step 1: Install Oracle VirtualBox

Oracle VirtualBox was installed successfully on the host machine and configured as the virtualization platform.

---

## Step 2: Create NAT Network

A dedicated NAT Network was created using the following settings:

```text
Network Name: NatNetwork
IPv4 Prefix: 10.0.0.0/24
DHCP: Enabled
```

### Screenshot

![NAT Network Configuration](Network%20settings.jpeg)

---

## Step 3: Import Kali Linux Virtual Machine

The official Kali Linux VirtualBox image was downloaded and imported successfully into Oracle VirtualBox.

### Screenshot

![Kali Linux VM](Kali%20Linux%20Image.jpeg)

---

## Step 4: Configure Kali Linux Networking

The network adapter was configured with a static IP address.

Configuration:

```text
IP Address: 10.0.0.2
Subnet Mask: /24
Gateway: 10.0.0.1
```

### Screenshot

![Network Configuration](Kali%20Linux%20Network%20settings.jpeg)

---

## Step 5: Configure Shared Resources

The following features were enabled:

- Shared Clipboard (Bidirectional)
- Drag and Drop (Bidirectional)
- Shared Folder (Downloads Folder)

These settings allow file and data sharing between the host machine and Kali Linux VM.

---

## Step 6: Verify Internet Connectivity

Internet connectivity was successfully verified.

Verification included:

- Accessing websites
- Updating repositories
- DNS resolution tests
- General network connectivity checks

Result:

✅ Internet Connectivity Successful

---

## Step 7: Create VM Snapshot

A recovery snapshot was created after completing the configuration.

Snapshot Name:

```text
Week1_Fresh_Kali_Lab
```

The snapshot can be restored if future lab activities affect the VM.

---

# 🔎 Lab Verification

| Test | Status |
|--------|---------|
| VirtualBox Installed | ✅ PASS |
| NAT Network Created | ✅ PASS |
| Kali Linux Imported | ✅ PASS |
| Static IP Configured | ✅ PASS |
| Internet Connectivity | ✅ PASS |
| Shared Clipboard Enabled | ✅ PASS |
| Drag and Drop Enabled | ✅ PASS |
| Shared Folder Configured | ✅ PASS |
| Snapshot Created | ✅ PASS |

---

# 📚 Skills Learned

Through this project I gained practical experience in:

- Virtualization Technology
- Oracle VirtualBox Administration
- Kali Linux Setup
- Virtual Networking
- NAT Network Configuration
- Linuxtual Environments

---

# 🚧 Challenges Encountered

## Challenge

Initial Kali Linux installation using an ISO image failed during the software installation process.

## Solution

The official Kali Linux VirtualBox image was downloaded and imported successfully, eliminating the need for manual installation.

---

# 🎓 Conclusion

The cybersecurity laboratory environment was successfully created using Oracle VirtualBox and Kali Linux.

The lab now provides a safe and controlled environment for future activities in cybersecurity, ethical hacking, vulnerability assessment, penetration testing, and network security studies as part of the NetworkWalks Cybersecurity Internship Program.

---

## 👨‍💻 Author

**Arnold Mumo Kilonzo**

BSc Information Technology Student  
University of Embu

Cybersecurity | Network Administration | IT Support | Generative AI
