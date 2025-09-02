# Linux Cheatsheet

A quick reference for essential Linux commands 🚀

---

## 1. File & Directory Management
- `pwd` → Show current working directory  
- `ls` → List files  
- `ls -la` → List all files with details  
- `cd /path` → Change directory  
- `mkdir myfolder` → Create a new directory  
- `rmdir myfolder` → Remove an empty directory  
- `rm -rf myfolder` → Remove a directory with files  
- `touch file.txt` → Create an empty file  
- `cp file.txt dir/` → Copy file to directory  
- `mv file.txt dir/` → Move file  
- `mv old.txt new.txt` → Rename file  
- `rm file.txt` → Delete file  

---

## 2. File Viewing & Editing
- `cat file.txt` → View file contents  
- `less file.txt` → Scroll through file  
- `head -n 10 file.txt` → First 10 lines  
- `tail -n 10 file.txt` → Last 10 lines  
- `nano file.txt` → Edit with Nano editor  
- `vim file.txt` → Edit with Vim editor  

---

## 3. File Permissions
- `ls -l` → View file permissions  
- `chmod 755 file.sh` → Change permissions (rwxr-xr-x)  
- `chown user:group file` → Change file owner  

---

## 4. Search & Find
- `find / -name file.txt` → Search for file  
- `grep "text" file.txt` → Search for text inside file  
- `grep -r "text" /dir` → Recursive search in directory  

---

## 5. System Info & Monitoring
- `whoami` → Current logged-in user  
- `uname -a` → Kernel + system info  
- `df -h` → Disk usage (human-readable)  
- `du -sh *` → Size of files/folders in dir  
- `free -h` → Memory usage  
- `uptime` → System uptime  
- `top` → Running processes  
- `htop` → Interactive process viewer  
- `ps aux` → List all processes  
- `kill -9 <PID>` → Kill process by PID  

---

## 6. Networking
- `ifconfig` → Network interfaces (deprecated, use `ip addr`)  
- `ip addr` → Show IP addresses  
- `ping google.com` → Test network  
- `curl http://url` → Get response from URL  
- `wget http://url` → Download file from URL  
- `netstat -tulnp` → Open ports & processes  

---

## 7. User Management
- `adduser newuser` → Add new user  
- `passwd newuser` → Change user password  
- `su - newuser` → Switch user  
- `who` → Show logged-in users  
- `groups` → Show user groups  

---

## 8. Archiving & Compression
- `tar -cvf archive.tar dir/` → Create tar archive  
- `tar -xvf archive.tar` → Extract tar archive  
- `gzip file.txt` → Compress file  
- `gunzip file.txt.gz` → Decompress file  

---

## 9. Shortcuts & Tricks
- `!!` → Run last command  
- `!abc` → Run last command starting with abc  
- `history` → Show command history  
- `clear` → Clear terminal  
- `alias ll='ls -la'` → Create alias

  ---

## 10. SSH (Secure Shell)
- `ssh user@host` → Connect to remote server  
- `ssh -p 2222 user@host` → Connect on custom port (e.g., 2222)  
- `ssh -i key.pem user@host` → Connect using private key  
- `scp file.txt user@host:/path` → Copy file to remote server  
- `scp user@host:/path/file.txt .` → Copy file from remote server  
- `rsync -avz file.txt user@host:/path` → Sync files (faster than scp)  
- `ssh-copy-id user@host` → Copy SSH key to server for passwordless login  
