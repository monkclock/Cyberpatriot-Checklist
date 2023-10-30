# Cyberpatriot-Checklist

1. Check ReadMe
2. Note down critical services
3. complete forensics questions
4. configure firefox
5. update critical services
6. update everything else
7. check for prohibited files .mp4, .mp3, .jpg, .txt, .png. .wav, etc be through because theres always something
8. remove prohibited software like wireshark, nmap, ophcrack, dsniff, wapiti
9. configure firewall
10. Change user passwords, add users, delete unauthorized users
11. check users password policies with chage -l "username"
12. configure login.defs
13. configure etc/pam.d/common-password for reference:https://www.debian.org/doc/manuals/securing-debian-manual/ch04s11.en.html
   may need to increase mininmun password length (password   [success=1 default=ignore]      pam_unix.so nullok obscure minlen=8 sha512)
 add line  (password required pam_pwhistory.so remember=5)
9.Update the '/etc/sudoers' or other sudo configuration files to remove or comment out lines utilizing the 'NOPASSWD' and '!authenticate' options.
14. turn off guest account in light dm
15. configure and harden critical services
