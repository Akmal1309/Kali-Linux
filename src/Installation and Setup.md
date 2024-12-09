# Kali Linux Installation and Setup Guide

This guide will help you install and configure Kali Linux for penetration testing and ethical hacking. Follow the steps below to get started!

---

## 1️⃣ System Requirements

Ensure your system meets the following requirements:

- **Processor:** 64-bit processor
- **RAM:** Minimum 4 GB (8 GB recommended)
- **Storage:** At least 20 GB of free disk space
- **Virtualization Software:** VMware Workstation/Player or VirtualBox

---

## 2️⃣ Downloading Kali Linux

1. Visit the [Kali Linux official website](https://www.kali.org/get-kali/).
2. Choose the version suitable for your setup:
   - **ISO file** for direct installation.
   - **Virtual Machine (VM)** images for use with VMware or VirtualBox.
3. Verify the downloaded file using the SHA256 checksum provided on the website.

---

## 3️⃣ Installing Kali Linux

### Option A: Installing on a Virtual Machine
1. Install and launch **VirtualBox** or **VMware** on your host system.
2. Create a new virtual machine:
   - Set the operating system type to **Linux** and version to **Debian (64-bit)**.
   - Allocate at least 2 processors and 4 GB of RAM.
   - Create a virtual hard disk with at least 20 GB of storage.
3. Attach the Kali Linux ISO or import the pre-built VM image.
4. Start the virtual machine and follow the on-screen installation prompts:
   - Select language, time zone, and keyboard layout.
   - Create a user account and set a password.
   - Configure disk partitioning (use guided partitioning if unsure).

### Option B: Installing on Bare Metal
1. Create a bootable USB drive using tools like **Rufus** or **Etcher**.
2. Insert the USB into your system and boot into the BIOS/UEFI.
3. Set the USB drive as the primary boot device.
4. Follow the installation prompts as described in Option A.

---

## 4️⃣ Post-Installation Configuration

1. **Update Kali Linux**:
   ```bash
   sudo apt update && sudo apt upgrade -y
   ```

2. **Install Additional Tools**:
   ```bash
   sudo apt install <tool-name>
   ```
   Example:
   ```bash
   sudo apt install nmap
   ```

3. **Configure Network Settings** (Optional):
   - Set up a static IP or configure a proxy if required.
   - Test network connectivity using:
     ```bash
     ping google.com
     ```

---

## 5️⃣ Troubleshooting Common Issues

- **Slow Virtual Machine Performance**:  
  Allocate more RAM and processors to the VM in your virtualization software settings.
  
- **Missing Tools**:  
  Some tools may not be pre-installed. Use the following command to install missing tools:
  ```bash
  sudo apt install kali-tools-top10
  ```

- **Network Issues**:  
  Ensure that network adapters in the VM settings are configured correctly (e.g., NAT or Bridged mode).

---

## 6️⃣ Next Steps

Once Kali Linux is installed and configured, you’re ready to explore its tools and features. Start by familiarizing yourself with the Linux command line and the Kali interface.

👉 [Go to Module 1: Introduction to Kali Linux](./README.md)

---

## Need Help?

If you encounter issues, check the [official documentation](https://www.kali.org/docs/) or post your question in the community forums.  
Happy Learning! 🎉
