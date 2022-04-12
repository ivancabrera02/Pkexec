# Pkexec
Privilege escalation
In Linux distributions there is a default SUID permission enabled in the "pkexec" binary that if not properly patched can allow an unprivileged user to easily become root.
Check -> which pkexec | xargs ls -l and if the "s" is found in the permissions, it may be vulnerable.
To solve it, simply remove the SUID permission.
To exploit this vulnerability we download the folder and run the .sh (if the system is vulnerable we should get a root shell).
