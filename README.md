# Linux
FTP, TFTP og Xen

# Installing TFTP on Ubuntu 16.04
sudo apt-get install tftpd-hpa
sudo vi /etc/default/tftpd-hpa

Change TFTP_DIRECTORY to "/srv/tftproot"
Change TFTP_OPTIONS to "--secure --create"

sudo mkdir /srv/tftproot
sudo chmod -R 777 /srv/tftproot
sudo chown -R tftp /srv/tftproot

sudo service tftpd-hpa restart
