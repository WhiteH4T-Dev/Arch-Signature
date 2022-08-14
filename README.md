<hr>

**Networks**

Enable the DHCP Server

    sudo systemctl enable --now dhcpcd.service
    
Show network configuration

    ifconfig

<hr>

**Solution**

signature from "Levon 'noptrix' Kayan (BlackArch Developer) &lt;noptrix@nullsecurity.net>" is invalid error

    rm -rf /etc/pacman.d/gnupg
    
    pacman-key --init
    
    pacman-key --populate archlinux blackarch
    
    pacman-key --update --keyserver keyserver.ubuntu.com
    
<hr>
