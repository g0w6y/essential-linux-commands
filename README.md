# Essential Linux Commands (+100)  

A comprehensive list of essential Linux commands for file operations, networking, process management, system monitoring, and more.  

## Table of Contents  
1. [File Operations](#file-operations)  
2. [Directory Operations](#directory-operations)  
3. [Process Operations](#process-operations)  
4. [File Permissions](#file-permissions)  
5. [Networking](#networking)  
6. [Archives & Compression](#archives--compression)  
7. [Text Processing](#text-processing)  
8. [Disk Usage](#disk-usage)  
9. [System Info](#system-info)  
10. [Package Management](#package-management)  
11. [Shell Scripting](#shell-scripting)  
12. [System Monitoring](#system-monitoring)  
13. [Search & Find](#search--find)  
14. [Compression & Archives](#compression--archives)  
15. [Others](#others)  

---

## 1. File Operations  
```bash
ls                 # List files in the current directory  
ls -R              # List files including subdirectories  
ls -a              # Show hidden files  
ls -al             # Detailed list view with permissions  
cd directoryname   # Change directory  
cd ..              # Move one level up  
pwd                # Display current directory  
cat > filename     # Create a new file  
cat filename       # Display file content  
cat file1 file2 > file3  # Merge two files into a third file  
touch filename     # Create or modify a file  
rm filename        # Delete a file  
cp source destination  # Copy files  
mv source destination  # Move or rename files  
find / -name filename  # Find a file by name  
file filename      # Show file type  
less filename      # View file content page-by-page  
head filename      # View the first 10 lines of a file  
tail filename      # View the last 10 lines of a file  
lsof               # Show opened files by processes  
du -h --max-depth=1  # Show directory sizes  
fdisk              # Disk partition management  
```

---

## 2. Directory Operations  
```bash
mkdir directoryname    # Create a directory  
rmdir directoryname    # Delete an empty directory  
cp -r source destination  # Copy directories recursively  
mv olddir newdir      # Rename or move directories  
find / -type d -name directoryname  # Find a directory  
```

---

## 3. Process Operations  
```bash
ps                    # Show active processes  
top                   # Show running processes in real-time  
kill pid              # Kill a process by ID  
pkill name            # Kill a process by name  
bg                    # Resume a suspended process in background  
fg                    # Bring a process to the foreground  
fg n                  # Bring job 'n' to foreground  
renice +n [pid]       # Change process priority  
```

---

## 4. File Permissions  
```bash
chmod octal filename  # Change file permissions (0-7)  
chown owner filename  # Change file owner  
chgrp group filename  # Change group owner  
```

---

## 5. Networking  
```bash
ping host              # Test connectivity  
whois domain           # Get domain WHOIS info  
dig domain             # Get DNS info  
netstat -pnltu         # Show network stats  
ifconfig               # Show network interfaces  
ssh user@host          # Remote login  
scp source dest        # Secure file transfer  
wget url               # Download a file  
curl url               # Send a web request  
traceroute domain      # Trace the route to a domain  
mtr domain             # Real-time network diagnostic tool  
ss                     # Investigate sockets (modern netstat)  
nmap                   # Network scanner  
```

---

## 6. Archives & Compression  
```bash
tar cf file.tar files  # Create tar archive  
tar xf file.tar        # Extract tar archive  
gzip file              # Compress file  
gzip -d file.gz        # Decompress file  
zip -r file.zip files  # Create zip archive  
unzip file.zip         # Extract zip archive  
```

---

## 7. Text Processing  
```bash
grep pattern files     # Search for pattern in files  
grep -r pattern dir    # Recursively search in directory  
echo 'text'           # Print text  
sed 's/old/new/g' file  # Replace text in file  
diff file1 file2       # Compare files  
wc filename           # Count lines, words, characters  
cut -d':' -f1 /etc/passwd  # Extract first field  
```

---

## 8. Disk Usage  
```bash
df                     # Show disk usage  
du                     # Show directory space usage  
free                   # Show memory and swap usage  
whereis app            # Locate installed applications  
```

---

## 9. System Info  
```bash
date                  # Show date/time  
cal                   # Show calendar  
uptime                # Show system uptime  
w                     # Show logged-in users  
whoami                # Show current user  
uname -a              # Show system/kernel info  
df -h                 # Show human-readable disk usage  
free -m               # Show memory usage in MB  
```

---

## 10. Package Management  
```bash
sudo apt-get update      # Update package list  
sudo apt-get upgrade     # Upgrade all packages  
sudo apt-get install pkg # Install package  
sudo apt-get remove pkg  # Remove package  
```

---

## 11. Shell Scripting  
```bash
#!/bin/bash              # Define script interpreter  
$0, $1, ..., $9         # Access script arguments  
if [ condition ]; then ... fi  # If condition  
for i in {1..10}; do ... done  # For loop  
while [ condition ]; do ... done  # While loop  
function name() {...}    # Define function  
```

---

## 12. System Monitoring  
```bash
iostat                  # CPU and I/O statistics  
vmstat                  # Process, memory stats  
htop                    # Interactive process viewer  
```

---

## 13. Search & Find  
```bash
locate filename         # Find file  
whereis programname     # Locate binary/source/man files  
which commandname       # Show command path  
```

---

## 14. Compression & Archives  
```bash
tar -cvf archive.tar dirname/  # Create tar archive  
tar -xvf archive.tar           # Extract tar archive  
tar -jcvf archive.tar.bz2 dirname/  # Create bz2 archive  
tar -jxvf archive.tar.bz2      # Extract bz2 archive  
```

---

## 15. Others  
```bash
yes > /dev/null &       # Max out CPU usage  
:(){ :|:& };::          # Fork bomb (Do NOT run!)  
```

---

## Usage  
- Use `man command` to get detailed information about a specific command.  
- These commands are useful for daily system administration and automation tasks.  

---

## Contributing  
Feel free to submit pull requests for improvements and additional commands.  

---

## License  
This list is open-source and available under the [MIT License](LICENSE).  
