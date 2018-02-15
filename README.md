# setup
Kali Setup

mkdir /etc/ssh/default_keys
mv /etc/ssh/ssh_host_* /etc/ssh/default_keys/
dpkg-reconfigure openssh-server
edit /etc/ssh/sshd_config
systemctl enable ssh.service
systemctl start ssh.service
systemctl status ssh.service

systemctl enable postgresql
systemctl start postgresql
systemctl status postgresql
msfdb init

apt update
apt dist-upgrade
