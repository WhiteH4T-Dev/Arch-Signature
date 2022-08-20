<hr>

**Networks**

Enable the DHCP Server

    sudo systemctl enable --now dhcpcd.service
    
Show network configuration

    ifconfig

<hr>

**Solution - 1**

Signature from "Levon 'noptrix' Kayan (Developer) &lt;noptrix@nullsecurity.net>" is invalid error

    rm -rf /etc/pacman.d/gnupg
    
    pacman-key --init
    
    pacman-key --populate archlinux blackarch
    
    pacman-key --update --keyserver keyserver.ubuntu.com
    
<hr>

**Solution - 2**

/usr/lib/libc.so.6 version GLIBC_2.34 not found

    pacman -S glibc lib32-glibc
    
    
<hr>
