# Linux Command Cheat Sheet 🐧

A curated list of **100 commonly used Linux commands**, organized by category for quick reference. Perfect for developers, system administrators, and Linux enthusiasts.

---

## Table of Contents
- [File & Directory Management](#file--directory-management)
- [Text Processing](#text-processing)
- [Network](#network)
- [System Monitoring](#system-monitoring)
- [Compression & Archiving](#compression--archiving)
- [Process Management](#process-management)
- [Permissions](#permissions)
- [SSH & Remote Access](#ssh--remote-access)
- [Scheduling & Automation](#scheduling--automation)
- [Miscellaneous](#miscellaneous)

---

## File & Directory Management
| Command | Description | Example |
|---------|-------------|---------|
| `pwd` | Print current working directory | `pwd` |
| `ls` | List directory contents | `ls -l` |
| `cd` | Change directory | `cd /home/user` |
| `mkdir` | Create a new directory | `mkdir new_folder` |
| `rm` | Remove files/directories | `rm file.txt` |
| `cp` | Copy files/directories | `cp file1.txt file2.txt` |
| `mv` | Move/rename files/directories | `mv oldname.txt newname.txt` |
| `touch` | Create empty file or update timestamp | `touch newfile.txt` |
| `chmod` | Change file permissions | `chmod 755 script.sh` |
| `chown` | Change file ownership | `chown user:user file.txt` |
| `chgrp` | Change file group ownership | `chgrp group file.txt` |
| `du` | Estimate file/directory space usage | `du -sh folder/` |
| `df` | Display disk space usage | `df -h` |
| `find` | Search for files/directories | `find /home -name "file.txt"` |
| `locate` | Find files by name (fast search) | `locate filename` |
| `updatedb` | Update file database for `locate` | `sudo updatedb` |

---

## Text Processing
| Command | Description | Example |
|---------|-------------|---------|
| `cat` | Display file contents | `cat file.txt` |
| `head` | Show first 10 lines of a file | `head file.txt` |
| `tail` | Show last 10 lines of a file | `tail file.txt` |
| `grep` | Search text using patterns | `grep "error" logfile.txt` |
| `awk` | Pattern scanning and text processing | `awk '{print $1}' file.txt` |
| `sed` | Stream editor for text manipulation | `sed 's/old/new/g' file.txt` |
| `diff` | Compare files line by line | `diff file1.txt file2.txt` |
| `sort` | Sort lines of text files | `sort file.txt` |
| `cut` | Extract sections from file lines | `cut -d':' -f1 /etc/passwd` |
| `wc` | Count lines, words, characters | `wc -l file.txt` |
| `tee` | Redirect output to multiple streams | `ls | tee output.txt` |

---

## Network
| Command | Description | Example |
|---------|-------------|---------|
| `ssh` | Securely connect to remote servers | `ssh user@remote_host` |
| `scp` | Securely copy files between systems | `scp file.txt user@remote_host:/path/` |
| `wget` | Download files from the web | `wget http://example.com/file.txt` |
| `curl` | Transfer data with URLs | `curl -O http://example.com/file.txt` |
| `ifconfig` | Configure network interfaces | `ifconfig eth0` |
| `ping` | Test network connectivity | `ping google.com` |
| `nslookup` | Query DNS records | `nslookup example.com` |
| `netstat` | Show network connections | `netstat -tulnp` |
| `ssh-keygen` | Generate SSH key pairs | `ssh-keygen -t rsa -b 2048` |
| `route` | Manage IP routing tables | `route -n` |
| `iptables` | Configure firewall rules | `sudo iptables -L` |
| `iftop` | Real-time network bandwidth monitor | `sudo iftop` |
| `nc` | Network tool for TCP/UDP connections | `nc -zv google.com 80` |

---

## System Monitoring
| Command | Description | Example |
|---------|-------------|---------|
| `top` | Monitor system processes in real-time | `top` |
| `ps` | Display running processes | `ps aux` |
| `kill` | Terminate processes by ID | `kill 1234` |
| `free` | Show memory usage | `free -m` |
| `uname` | Display system information | `uname -a` |
| `uptime` | Show system uptime and load | `uptime` |
| `who` | List logged-in users | `who` |
| `date` | Display/set system date/time | `date` |
| `cal` | Show calendar | `cal` |
| `lscpu` | Display CPU architecture details | `lscpu` |
| `lshw` | List hardware configuration | `sudo lshw` |
| `lspci` | List PCI devices | `lspci` |
| `lsusb` | List USB devices | `lsusb` |
| `sar` | System activity reporter | `sar -u 5 10` |
| `lsof` | List open files and processes | `lsof -i` |

---

## Contributing
Contributions welcome! 🎉 Please open an issue or submit a pull request for improvements.

## License
This project is licensed under the MIT License.

---

This README now includes examples for every command!

