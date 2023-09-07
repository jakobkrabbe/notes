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
Nameserver reset:
sudo nano /etc/resolv.conf

# nameserver 127.0.0.53
nameserver 8.8.8.8
```
