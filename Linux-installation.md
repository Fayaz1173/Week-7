## **1. VirtualBox Setup**

1. Open VirtualBox → Click **New**
2. Name: `LinuxVM`
3. Type: **Linux**, Version: **Ubuntu (64-bit)**
4. Memory size: **2048–4096 MB**
5. Hard disk: **Create a virtual hard disk now → VDI → Dynamically allocated → 20 GB**
6. Finish VM creation

---

## **2. Load Linux ISO**

1. Select your VM → **Settings → Storage**
2. Click **Empty** under Controller: IDE → Click the CD icon → **Choose a disk file** → Select your downloaded Linux ISO
3. Click **OK**

---

## **3. Boot & Install Linux**

1. Start VM → It will boot from ISO
2. Select **“Install Ubuntu”** (or your Linux choice)
3. Follow installation prompts:
    - Language → Keyboard layout → Updates
    - Disk setup: **Erase disk and install Linux** (safe inside VM)
    - Set username and password
4. Wait for installation to complete → Reboot VM

---

## **4. Post-Installation Configuration**

1. Remove the ISO from virtual drive (Settings → Storage → remove ISO)
2. Update system packages:

```bash
sudo apt update && sudo apt upgrade -y

```

1. Optional: Install **Guest Additions** for better performance:
    - Devices → Insert Guest Additions CD image
    - Follow instructions in VM terminal

---

## **5. Recommended VM Settings for Safety**

- **Snapshots:** Take a snapshot before experimenting → allows you to restore VM if something breaks
- **Network:** Use NAT for Internet, Host-Only if you want isolated network
- **Shared folders / clipboard:** Disable or limit for security
- **Memory & CPU:** Adjust to balance host performance and VM speed
