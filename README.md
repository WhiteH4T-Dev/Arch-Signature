![](https://c.tenor.com/JIS_KDKKsgYAAAAM/guaton-computadora.gif)

This was created for Arch Linux users who have the same problems.
Once you've completed the steps below, your system should function properly. 

<hr>

**Networks**

Enable the DHCP Server

    sudo systemctl enable --now dhcpcd.service
    
Show network configuration

    ifconfig
    
<hr>

**Connect to Wireless Network**

    iwctl
    device list
    station <interface> scan
    station <interface> get-networks
    station <interface> connect <network_name>
    **Type in your password**
    exit

<hr>

**Solution - 1**

Waiting for IWD to start...
   
    systemctl enable --now iwd

<hr>

**Solution - 2**

Signature from "Levon 'noptrix' Kayan (Developer) &lt;noptrix@nullsecurity.net>" is invalid error

    rm -rf /etc/pacman.d/gnupg
    
    pacman-key --init
    
    pacman-key --populate archlinux blackarch
    
    pacman-key --update --keyserver keyserver.ubuntu.com
    
<hr>

**Solution - 3**

/usr/lib/libc.so.6 version GLIBC_2.34 not found

    pacman -S glibc lib32-glibc
    
    
<hr>
