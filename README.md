# Cyberpatriot-Checklist

1. Check ReadMe
2. Note down critical services
3. complete forensics questions
4. configure firefox
5. update critical services
6. update everything else
7. check for security updates
8. check for prohibited files .mp4, .mp3, .jpg, .txt, .png. .wav, etc be through because theres always something
9. check for bad services
10. remove prohibited software like wireshark, nmap, ophcrack, dsniff, wapiti
11. configure firewall
12. Change user passwords, add users, delete unauthorized users
13. search for hidden users in group, passwd, and shadow files
14. check users password policies with chage -l "username"
15. configure login.defs
16. configure etc/pam.d/common-password for reference:https://www.debian.org/doc/manuals/securing-debian-manual/ch04s11.en.html
   may need to increase mininmun password length (password   [success=1 default=ignore]      pam_unix.so nullok obscure minlen=8 sha512)
 add line  (password required pam_pwhistory.so remember=5)
9.Update the '/etc/sudoers' or other sudo configuration files to remove or comment out lines utilizing the 'NOPASSWD' and '!authenticate' options.
17. turn off guest account in light dm
18. configure and harden critical services
19. install clamav and scan:  https://docs.e2enetworks.com/security/bestpractice/clamav_scan.html

things to try after doing all of those things: 
1. prevent normal users from using dmseg:  sudo sysctl -w kernel.dmesg_restrict=1
2. disable snmpd
3. disable ircd
4. double check prohibited apps
5. double check critical service hardening
