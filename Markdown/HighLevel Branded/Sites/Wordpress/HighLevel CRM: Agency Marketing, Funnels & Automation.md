**Date Updated:** 2025-06-24T23:19:58.000Z

This article will guide you through setting up SSH access for your WordPress hosting environment, allowing you to securely manage your website via command line tools like WP-CLI. You’ll learn how to generate SSH keys, add them to your hosting dashboard, and connect to your server securely on different operating systems.

  
**TABLE OF CONTENTS**

* [What is SSH and Why Use It?](#What-is-SSH-and-Why-Use-It?)
* [Key Benefits of SSH Access](#Key-Benefits-of-SSH-Access)
* [How To Create Your SSH Key](#How-To-Create-Your-SSH-Key)  
   * [On macOS](#On-macOS)  
   * [On Linux](#On-Linux)  
   * [On Windows](#On-Windows)
* [How To Add Your SSH Key to the Hosting Dashboard](#How-To-Add-Your-SSH-Key-to-the-Hosting-Dashboard)
* [How To Connect to Your Server via SSH](#How-To-Connect-to-Your-Server-via-SSH)
* [Common WP-CLI Commands](#Common-WP-CLI-Commands)
* [Managing SSH Keys](#Managing-SSH-Keys)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

  
---

  
# **What is SSH and Why Use It?**

  
SSH (Secure Shell) is a secure protocol that enables encrypted connections to your server. It’s ideal for advanced users who want direct access to server resources, offering greater control and automation possibilities for WordPress management.

  
_![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155048810461/original/VtpVJotbnt8DU4zjBDiC30ZKLAKDbAKMkQ.png?1750786796)_

_![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155048810470/original/2El18UwuiFIjXWaxfP07doVCTzUyG3G2kw.png?1750786804)_  

  
# **Key Benefits of SSH Access**

  
SSH access offers several key advantages that improve server management and site security:

* Enables use of **WP-CLI** for faster, scriptable WordPress management
* Provides secure, encrypted server connections
* Allows direct file operations without needing FTP
* Facilitates automation and deployment workflows
* Supports multi-user, key-based authentication for teams
* Enhances security through passwordless, key-based login

  
# **How To Create Your SSH Key**

  
Creating an SSH key ensures only authorized devices can connect to your server. Follow the steps for your specific operating system.

  
## **On macOS**

  
You can quickly generate and copy your SSH key using Terminal.

1. Open **Terminal**.
2. Run: ssh-keygen -t rsa
3. Press Enter through all prompts (no password required).
4. Copy your key: pbcopy < \~/.ssh/id\_rsa.pub

  
_![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155048810476/original/eMqljVaWPFzV23f73ONEj6KS6c2IWoklXA.png?1750786818)_

  
## **On Linux**

  
Generating and copying your SSH key is simple and secure on Linux.

1. Open **Terminal**.
2. Run: ssh-keygen -t rsa
3. Accept defaults by pressing Enter.
4. Install xclip if needed:  
   * Ubuntu: sudo apt install xclip  
   * Arch: sudo pacman -S xclip  
   * Fedora/CentOS: sudo yum -y install xclip
5. Copy key: cat \~/.ssh/id\_rsa.pub | xclip -sel clip
  
  
## **On Windows**

  
Windows users can create SSH keys using PowerShell.

1. Open **PowerShell**.
2. Run: ssh-keygen.exe -t rsa
3. Press Enter through prompts.
4. Copy key: Get-Content .ssh\\id\_rsa.pub | Set-Clipboard
  
  
# **How To Add Your SSH Key to the Hosting Dashboard**

  
Adding your SSH key authorizes your device for server access.

1. Log in to your hosting dashboard.
2. Navigate to **Advanced Settings > Server Settings**.
3. Enable SSH Access.
4. Go to **SSH Keys Manager** → click **Import New Key**.
5. Paste your public key.
6. Name your key (e.g. “Jane’s MacBook”).
7. Click **Import** — system will authorize your key.

  
_![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155048810523/original/fW5WGEixKbTe0XP5NBYxIe-VaM-krrPoQ.png?1750786855)_

  
# **How To Connect to Your Server via SSH**

  
Connecting allows you to use terminal commands on your server.

1. Get your **Host/IP** and **Username** from the dashboard.
2. Open terminal.
3. Run: ssh yourusername@yourhostip
4. Confirm first-time connection with yes.
5. Navigate to your WordPress directory:  
   * cd public\_html

  
_![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155048810528/original/I5rpgnCRvGK9MDHAzdRdlw9XyTBwQg8JGA.png?1750786866)_

  
# **Common WP-CLI Commands**

  
These commands help manage your WordPress site efficiently:

* List plugins: wp plugin list
* Clear cache: wp cache flush
* Purge CDN cache: wp cdn purge

  
# **Managing SSH Keys**

  
You can manage keys for better security and flexibility:

* **Delete unused keys** anytime via SSH Keys Manager.
* **Add keys for other devices/team members**.
* **Rotate keys regularly** for enhanced security.

---

# Frequently Asked Questions

Q: What happens if I lose my private key? You’ll need to generate a new key pair and re-add the public key.

Q: Can I use a password instead of a key? No, key-based authentication is required for SSH on this hosting platform.

Q: How do I revoke access for a stolen device? Delete the corresponding key from SSH Keys Manager immediately.

Q: Is SSH access available on all plans? Please check your hosting plan details — some plans may not include SSH.