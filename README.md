# Ubuntu Guide

---

## What is Ubuntu?
Ubuntu is a free and open-source Linux-based operating system developed by Canonical. It is one of the most popular Linux distributions, widely used for personal, professional, and server environments. Ubuntu is known for its ease of use, security, and large community support.

---

## Why Use Ubuntu?

1. **Open Source & Free** - Ubuntu is completely free and open source, making it an attractive option for individuals and businesses.
2. **User-Friendly Interface** - Ubuntu offers a clean and intuitive interface, making it accessible even for beginners.
3. **Security & Stability** - With regular security updates and a strong development community, Ubuntu is one of the most secure operating systems.
4. **Software Availability** - It supports a vast repository of open-source applications and tools.
5. **Customization & Flexibility** - Users can customize Ubuntu as per their requirements, from UI themes to system configurations.
6. **Community Support** - A large community and extensive documentation make troubleshooting easier.
7. **Compatibility with Cloud & Servers** - Ubuntu is widely used in cloud computing and server management due to its robustness.
8. **Performance & Efficiency** - Ubuntu is optimized for performance and is widely used in lightweight computing environments.
9. **Developer-Friendly** - Ubuntu supports a range of development tools, making it a preferred OS for developers and engineers.

---

## Different Versions of Ubuntu

Ubuntu has different versions catering to various needs:

1. **Ubuntu Desktop** - The standard version for personal use, featuring a GUI and pre-installed applications.
2. **Ubuntu Server** - Designed for server environments, offering optimized performance and security features.
3. **Ubuntu Core** - A minimal, containerized version of Ubuntu for IoT and embedded devices.
4. **Ubuntu Studio** - A version tailored for multimedia production, including audio, video, and graphics tools.
5. **Kubuntu, Xubuntu, Lubuntu** - Lightweight variants with different desktop environments for varied user experiences.

---


## Basic Linux Commands

### 1. `pwd` – Print current working directory
```sh
pwd
```
**Example Output:**
```
/home/user
```

### 2. `ls` – List files in a directory
```sh
ls
```
**Example Output:**
```
documents downloads pictures music
```

### 3. `ls -l` – Detailed list of files
```sh
ls -l
```
**Example Output:**
```
drwxr-xr-x 2 user user 4096 Mar 27 10:00 Documents
-rw-r--r-- 1 user user  123 Mar 27 10:05 file.txt
```

### 4. `ls -a` – Show hidden files
```sh
ls -a
```
**Example Output:**
```
.  ..  .bashrc  .profile  Documents  Downloads
```

### 5. `cd <directory>` – Change directory
```sh
cd Documents
```

### 6. `cd ..` – Move up one level
```sh
cd ..
```

### 7. `mkdir <dir>` – Create a new directory
```sh
mkdir my_folder
```

### 8. `rmdir <dir>` – Remove an empty directory
```sh
rmdir my_folder
```

### 9. `rm <file>` – Delete a file
```sh
rm file.txt
```

### 10. `rm -r <dir>` – Remove a directory and its contents
```sh
rm -r my_folder
```

### 11. `cp <source> <destination>` – Copy files
```sh
cp file.txt /home/user/Documents/
```

### 12. `cp -r <source> <destination>` – Copy directories
```sh
cp -r folder1 folder2
```

### 13. `mv <source> <destination>` – Move or rename files
```sh
mv oldname.txt newname.txt
```

### 14. `touch <file>` – Create an empty file
```sh
touch newfile.txt
```

### 15. `cat <file>` – Show file contents
```sh
cat file.txt
```

### 16. `less <file>` – View file page-wise
```sh
less largefile.txt
```

### 17. `more <file>` – View file with pagination
```sh
more file.txt
```

### 18. `head <file>` – View first 10 lines
```sh
head file.txt
```

### 19. `tail <file>` – View last 10 lines
```sh
tail file.txt
```

### 20. `tail -f <file>` – View file changes in real-time
```sh
tail -f logfile.log
```

### 21. `echo "Hello World"` – Print text
```sh
echo "Hello World"
```

### 22. `clear` – Clear the terminal
```sh
clear
```

### 23. `history` – Show command history
```sh
history
```

### 24. `uptime` – Show system uptime
```sh
uptime
```

### 25. `whoami` – Show the current user
```sh
whoami
```

### 26. `who` – Show logged-in users
```sh
who
```

### 27. `w` – Show detailed user activity
```sh
w
```

### 28. `date` – Show system date
```sh
date
```

### 29. `cal` – Display a calendar
```sh
cal
```

### 30. `df -h` – Show disk space usage
```sh
df -h
```

### 31. `du -sh <dir>` – Show directory size
```sh
du -sh Documents
```

### 32. `lsblk` – List block devices
```sh
lsblk
```

### 33. `blkid` – Display UUID of partitions
```sh
blkid
```

### 34. `mount /dev/sdb1 /mnt` – Mount a drive
```sh
mount /dev/sdb1 /mnt
```

### 35. `umount /mnt` – Unmount a drive
```sh
umount /mnt
```

### 36. `free -h` – Show memory usage
```sh
free -h
```

### 37. `uname -a` – Show system information
```sh
uname -a
```

### 38. `hostname` – Display system hostname
```sh
hostname
```

### 39. `uptime` – Show system uptime
```sh
uptime
```

### 40. `env` – Show environment variables
```sh
env
```

### 41. `export VAR=value` – Set an environment variable
```sh
export MY_VAR=hello
```

### 42. `alias ll='ls -lah'` – Create a command alias
```sh
alias ll='ls -lah'
```

### 43. `unalias ll` – Remove an alias
```sh
unalias ll
```

### 44. `passwd` – Change password
```sh
passwd
```

### 45. `exit` – Logout from terminal
```sh
exit
```

### 46. `shutdown -h now` – Shutdown the system
```sh
shutdown -h now
```

### 47. `reboot` – Restart the system
```sh
reboot
```

### 48. `sleep 5` – Wait for 5 seconds
```sh
sleep 5
```

### 49. `time <command>` – Measure execution time of a command
```sh
time ls
```

### 50. `man <command>` – Show the manual for a command
```sh
man ls
```

### **File Permissions and Ownership Commands**

| Command | Description | Example |
|---------|-------------|---------|
| `chmod 777 <file>` | Full permissions | `$ chmod 777 myscript.sh` |
| `chmod 755 <file>` | Read & execute for all, write for owner | `$ chmod 755 script.sh` |
| `chown user:group <file>` | Change file ownership | `$ chown john:dev team.txt` |
| `ls -l` | View file permissions | `$ ls -l` |
| `stat <file>` | Get detailed file information | `$ stat myfile.txt` |
| `lsattr` | List file attributes | `$ lsattr` |
| `setfacl -m u:user:rwx <file>` | Set ACL for a user | `$ setfacl -m u:john:rwx file.txt` |

---

### **User Management Commands**

| Command | Description | Example |
|---------|-------------|---------|
| `whoami` | Show current user | `$ whoami` → `user` |
| `id` | Display user ID | `$ id` |
| `who` | Show all logged-in users | `$ who` |
| `adduser <username>` | Create a new user | `$ adduser john` |
| `passwd <username>` | Set a user's password | `$ passwd john` |
| `deluser <username>` | Delete a user | `$ deluser john` |
| `groupadd <groupname>` | Create a new group | `$ groupadd developers` |
| `groups <username>` | Show user groups | `$ groups john` |
| `su <username>` | Switch user | `$ su john` |
| `sudo su` | Switch to root | `$ sudo su` |

---

### **Networking Commands**

| Command | Description | Example |
|---------|-------------|---------|
| `ping <host>` | Check connectivity | `$ ping google.com` |
| `traceroute <host>` | Trace route to a host | `$ traceroute google.com` |
| `nslookup <host>` | DNS lookup | `$ nslookup google.com` |
| `curl -I <URL>` | Fetch HTTP headers | `$ curl -I https://example.com` |
| `wget <URL>` | Download a file | `$ wget https://example.com/file.zip` |
| `netstat -tulnp` | Show open ports | `$ netstat -tulnp` |
| `ip addr show` | Show IP addresses | `$ ip addr show` |
| `hostname -I` | Show IP address | `$ hostname -I` |

---

## Conclusion
Ubuntu is a powerful and versatile operating system with strong community support. Whether you are a beginner or an advanced user, mastering these commands will enhance your Linux experience. 🚀

---

## 🌟 Contributing
If you have suggestions or improvements, feel free to create a pull request!

---

## 📜 License
This project is licensed under the MIT License.

