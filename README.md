# Helpful Tricks for Linux

---

## Backup Ub16 presentation machine via USB thumb drive

Setup

   1. Boot from USB drive

   1. Enable password-less sudo   
      ```
      sudo visudo
      ```
      (append: `ubuntu ALL=(ALL) NOPASSWD: ALL ` to the text of sudoers)

   1. Set a password for login / screen lock
      ```
      sudo passwd ubuntu
      ```
   1. Enable screen lock (for suspend/reboot protection)
      ```
      gsettings set org.gnome.desktop.lockdown disable-lock-screen 'false'
      ```
