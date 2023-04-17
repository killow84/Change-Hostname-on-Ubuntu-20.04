# Change-Hostname-on-Ubuntu-20.04
How to Change Hostname on Ubuntu 20.04
```
sudo hostname new-hostname
```
## Change Hostname on Ubuntu 20.04 (No Reboot Required)
### Step 1: Use set-hostname to Change the Hostname
```
hostnamectl set-hostname new-hostname
```
### Step 2: Use hostnamectl to Confirm the Change
```
sudo hostnamectl set-hostname
```
### Step 3: Change the Pretty Hostname (Optional)
```
hostnamectl set-hostname "new-hostname" --pretty
```
## Change Hostname on Ubuntu 20.04 – Alternative Method (Reboot Required)
Another way to permanently change the hostname is by editing two configuration files:
```
/etc/hostname
/etc/hosts
```
### The changes take effect immediately after system reboot.

### Step 1: Open /etc/hostname and Change the Hostname
Edit the file with a text editor of your choice. In this example, we will be using the Vim editor:
```
sudo vi /etc/hostname
```
### Step 2: Open /etc/hosts and Change the Hostname
Now edit the /etc/hosts file in the same way.
```
sudo vi /etc/hosts
```
### Step 3: Reboot the System
```
sudo systemctl reboot
```
