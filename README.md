# Linux Command Cheat Sheet 🐧

A curated list of **100 commonly used Linux commands** with examples, organized by category for quick reference. Perfect for developers, system administrators, and Linux enthusiasts.

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
| `ls` | List directory contents | `ls -l` (detailed view) |
| `cd` | Change directory | `cd /var/www` |
| `mkdir` | Create a new directory | `mkdir project` |
| `rm` | Remove files/directories | `rm -r folder` (recursive delete) |
| `cp` | Copy files/directories | `cp file.txt /backup/` |
| `mv` | Move/rename files/directories | `mv oldname.txt newname.txt` |
| `touch` | Create empty file or update timestamp | `touch test.txt` |
| `chmod` | Change file permissions | `chmod 755 script.sh` |
| `chown` | Change file ownership | `chown user:group file.txt` |
| `chgrp` | Change file group ownership | `chgrp developers file.txt` |
| `du` | Estimate file/directory space usage | `du -sh /home` (human-readable) |
| `df` | Display disk space usage | `df -h` (human-readable) |
| `find` | Search for files/directories | `find . -name "*.log"` |
| `locate` | Find files by name (fast search) | `locate httpd.conf` |
| `updatedb` | Update file database for `locate` | `sudo updatedb` |

---

## Text Processing
| Command | Description | Example |
|---------|-------------|---------|
| `cat` | Display file contents | `cat file.txt` |
| `head` | Show first 10 lines of a file | `head -n 20 file.txt` |
| `tail` | Show last 10 lines of a file | `tail -f /var/log/syslog` (follow logs) |
| `grep` | Search text using patterns | `grep "error" logs.txt` |
| `awk` | Pattern scanning and text processing | `awk '{print $1}' data.csv` |
| `sed` | Stream editor for text manipulation | `sed 's/old/new/g' file.txt` |
| `diff` | Compare files line by line | `diff file1.txt file2.txt` |
| `sort` | Sort lines of text files | `sort -r file.txt` (reverse order) |
| `cut` | Extract sections from file lines | `cut -d',' -f1 names.csv` |
| `wc` | Count lines, words, characters | `wc -l file.txt` (line count) |
| `tee` | Redirect output to multiple streams | `echo "test" | tee log.txt` |

---

## Network
| Command | Description | Example |
|---------|-------------|---------|
| `ssh` | Securely connect to remote servers | `ssh user@192.168.1.10` |
| `scp` | Securely copy files between systems | `scp file.txt user@remote:/path` |
| `wget` | Download files from the web | `wget https://example.com/file.zip` |
| `curl` | Transfer data with URLs | `curl -O https://example.com/data.json` |
| `ifconfig` | Configure network interfaces | `ifconfig eth0` |
| `ping` | Test network connectivity | `ping google.com` |
| `nslookup` | Query DNS records | `nslookup example.com` |
| `netstat` | Show network connections | `netstat -tuln` (listening ports) |
| `ssh-keygen` | Generate SSH key pairs | `ssh-keygen -t ed25519` |
| `route` | Manage IP routing tables | `route -n` |
| `iptables` | Configure firewall rules | `iptables -L` (list rules) |
| `iftop` | Real-time network bandwidth monitor | `iftop -i eth0` |
| `nc` | Network tool for TCP/UDP connections | `nc -zv 127.0.0.1 80` (port check) |

---

## System Monitoring
| Command | Description | Example |
|---------|-------------|---------|
| `top` | Monitor system processes in real-time | `top` |
| `ps` | Display running processes | `ps aux` |
| `kill` | Terminate processes by ID | `kill 1234` |
| `free` | Show memory usage | `free -h` (human-readable) |
| `uname` | Display system information | `uname -a` (all details) |
| `uptime` | Show system uptime and load | `uptime` |
| `who` | List logged-in users | `who` |
| `date` | Display/set system date/time | `date "+%Y-%m-%d"` |
| `cal` | Show calendar | `cal 2023` |
| `lscpu` | Display CPU architecture details | `lscpu` |
| `lshw` | List hardware configuration | `sudo lshw -short` |
| `lspci` | List PCI devices | `lspci | grep VGA` |
| `lsusb` | List USB devices | `lsusb` |
| `sar` | System activity reporter | `sar -u 2 5` (CPU usage) |
| `lsof` | List open files and processes | `lsof -i :80` (port 80 usage) |

---

## Compression & Archiving
| Command | Description | Example |
|---------|-------------|---------|
| `tar` | Create/extract tar archives | `tar -czvf archive.tar.gz files/` |
| `gzip` | Compress files | `gzip file.txt` |
| `gunzip` | Decompress gzipped files | `gunzip file.txt.gz` |
| `zip` | Create zip archives | `zip -r archive.zip folder/` |
| `unzip` | Extract zip archives | `unzip archive.zip` |
| `rsync` | Sync files/directories efficiently | `rsync -av /source /destination` |

---

## Process Management
| Command | Description | Example |
|---------|-------------|---------|
| `nohup` | Run commands immune to hangups | `nohup ./long_script.sh &` |
| `lsof` | List open files and processes | `lsof /var/log/syslog` |

---

## Permissions
| Command | Description | Example |
|---------|-------------|---------|
| `chmod` | Modify file permissions | `chmod 644 file.txt` |
| `chown` | Change file owner | `sudo chown root:root /etc/file` |
| `chgrp` | Change file group | `chgrp www-data index.html` |

---

## SSH & Remote Access
| Command | Description | Example |
|---------|-------------|---------|
| `ssh` | Secure Shell connection | `ssh user@hostname` |
| `scp` | Secure file copy | `scp user@remote:/file /local/path` |
| `ssh-keygen` | Generate SSH keys | `ssh-keygen -t rsa -b 4096` |

---

## Scheduling & Automation
| Command | Description | Example |
|---------|-------------|---------|
| `crontab` | Schedule recurring tasks | `crontab -e` (edit cron jobs) |

---

## Miscellaneous
| Command | Description | Example |
|---------|-------------|---------|
| `man` | Display command manual pages | `man ls` |
| `which` | Locate command executable | `which python` |
| `history` | Show command history | `history 10` (last 10 commands) |
| `sudo` | Execute commands as superuser | `sudo apt update` |
| `su` | Switch user account | `su - username` |
| `alias` | Create command shortcuts | `alias ll='ls -la'` |
| `source` | Execute commands from a file | `source ~/.bashrc` |
| `shutdown` | Shutdown the system | `shutdown -h now` |
| `reboot` | Reboot the system | `reboot` |
| `halt` | Stop the system | `halt` |

---

## Contributing
Contributions welcome! 🎉 Please open an issue or submit a pull request for improvements.

## License
This project is licensed under the MIT License.  
Copyright © 2023 [Your Name]
