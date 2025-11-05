# Chen_Cyber
Only Documenting my CyberSecurity Learning

#TRYHACKME DOCUMENTATION
Linux logging for COC PAGE:
Logs are kept in /var/log/ folder by default and are usually stored in plain text
The top three log sources for SOC are auth.log, app-specific logs, and runtime logs
Bash history is unreliable for SOC; better use auditd or an alternative solution
ausearch -i -k proc_wget
