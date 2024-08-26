# notes
Personal notes but no secrets!

```
Dirvish back-up: 
Look for lock-file! If found, remove!

la -ls /srv/backup/*/dirvish/lock_file
sudo rm -r /srv/backup/*/dirvish/lock_*
ls | grep "Backup-begin:" /srv/backup/*/20230905/summary
ls | grep "Backup-complete:" /srv/backup/*/20230905/summary
```

```
How to Use the Tail Command
https://www.linode.com/docs/guides/how-to-use-tail/
```
```
Mirror sites:
wget https://ftp.lysator.liu.se/ubuntu-releases/22.04/ubuntu-22.04.3-live-server-amd64.iso

How To Set Permanent DNS Nameservers in Ubuntu
https://www.tecmint.com/set-permanent-dns-nameservers-in-ubuntu-debian/
$ sudo apt update
$ sudo apt install resolvconf

Nameserver reset:
sudo nano /etc/resolv.conf

# nameserver 127.0.0.53
nameserver 8.8.8.8
search vertel.se

# No IP is given
https://serverfault.com/questions/1087923/how-to-fix-ubuntu-not-getting-ip-address-on-hyper-v
1. sudo dhclient eth0
1. sudo dhclient ens1
2. sudo nano /etc/netplan/01-network-manager-all.yaml
3. sudo netplan apply
4. Clean the disk! https://www.esds.co.in/kb/how-to-clean-up-ubuntu-server/

nameserver 8.8.8.8
options edns0 trust-ad
search vertel.se
vertel@gluu20:~$ sudo nano /etc/apt/sources.list
vertel@gluu20:~$ sudo apt update

Swap-off
sudo swapoff -a
sudo nano /etc/sysctl.conf
sudo rm -r swapoff.img


List the most recent log
jakob@bart:/var/log$ ls -lart

Install requirements
/usr/share/odoo-crm/$ sudo pip3 install -r requirements.txt 

 Install 'jingtrang' for more precise and useful validation messages.
pip3 install jingtrang



# Permissions for /etc/netplan/01-network-manager-all.yaml are too open. Netplan configuration should NOT be accessible by others.
1. chmod 600 /etc/netplan/your_config_file.yaml
... should solve your problem. Do this for every netplan file that was listed in the warnings.

```
