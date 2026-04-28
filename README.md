# Self_Hosted
How to setup my Home self hosted bits & bobs

# Mounting NAS to ubuntu
Below to Mount NAS
sudo mount -t cifs -o vers=2.0,credentials=/home/dockeradm/.smbcreds //<IPADDRESS>/Media /mnt/NAS

Below to mount NAS automagically using fstab
//<IPADDRESS>/Media /mnt/NAS cifs credentials=/home/dockeradm/.smbcreds,vers=2.0,iocharset=utf8 0 0

Both option above use user/password stored in smbcreds in following format
username=USERNAME
password=PASSWORD
