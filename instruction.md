#Server system
Ubuntu 12&14

##LDAP
[Reference](https://www.digitalocean.com/community/tutorials/how-to-authenticate-client-computers-using-ldap-on-an-ubuntu-12-04-vps)
1. Install LDAP client
```bash
$ sudo apt-get install libpam-ldap nscd
ldap://LDAP-server-IP-Address
base dn: dc=pekka,dc=iis,dc=sinica,dc=edu,dc=tw
LDAP version to use: 3
Make local root Database admin: Yes
Does the LDAP database require login? No
LDAP account for root: uid=root,cn=users,dc=pekka,dc=iis,dc=sinica,dc=edu,dc=tw
password: please_ask_administrator
$ sudo dpkg-reconfigure ldap-auth-config
```
2.  Setting authentication files
```bash
$ vim /etc/nsswitch.conf
passwd:         files ldap
group:          files ldap
shadow:         files ldap
$ vim /etc/pam.d/common-session (PAM configuration)
session required    pam_mkhomedir.so skel=/etc/skel umask=0022
```

3. Restart service
```bash
$ sudo /etc/init.d/nscd restart
$ vim /etc/sudoers (Permission configuration)
 %administrators ALL=(ALL) ALL
```

4. Integration with ZH
```bash
$ vim /etc/ldap.conf
nss_override_attribute_value loginShell /usr/bin/zsh
```
## NFS
[Reference](https://www.digitalocean.com/community/tutorials/how-to-set-up-an-nfs-mount-on-ubuntu-12-04)

1. Install NFS
```bash
$ sudo apt-get install nfs-common portmap
```
2. configure
```bash
$ mkdir /tempHome, /corpus /tools
$ vim /etc/fstab
$ mount -a
```

