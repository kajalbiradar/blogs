---
title: "Linux Cheat Sheet: Essential Commands🐧🚀"
datePublished: Thu Aug 03 2023 18:12:20 GMT+0000 (Coordinated Universal Time)
cuid: clkvh5702000009lbbc8gf5vm
slug: linux-cheat-sheet-essential-commands
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1691079972163/f3437ec7-28fb-4609-86dc-2b48b3ca569e.webp
tags: linux, devops, cheatsheet, 90daysofdevops, trainwithshubham

---

## 🌟 Introduction

Linux, the powerful and versatile operating system, is the cornerstone of modern computing. Whether you're a beginner or a seasoned user, understanding essential Linux commands can significantly enhance your productivity and efficiency. This cheat sheet provides a handy reference for navigating through basic commands, file permissions, process management, networking, environment variables, text editing with Vi, user management, file compression, and system information.

## 📂 **Basic Commands**

* `pwd`: Show the present working directory.
    
* `ls`: List files and directories in the current directory.
    
* `cd`: Change directory. Use `cd ..` to go up one level.
    
* `mkdir`: Create a new directory. Example: `mkdir folder_name`.
    
* `rmdir`: Remove a directory. Example: `rmdir folder_name` (only if it's empty).
    
* `touch`: Create an empty file. Example: `touch filename`.
    
* `cp`: Copy files or directories. Example: `cp source_file destination`.
    
* `mv`: Move or rename files or directories. Example: `mv old_filename new_filename`.
    
* `rm`: Remove files or directories. Example: `rm filename`.
    
* `cat`: Display the contents of a file.
    
* `less`: Display file content interactively, page by page.
    
* `head`: Display the beginning of a file (default: first 10 lines).
    
* `tail`: Display the end of a file (default: last 10 lines).
    
* `grep`: Search for a pattern in a file. Example: `grep 'pattern' filename`.
    
* `find`: Search for files and directories. Example: `find /path/to/search -name "filename"`.
    

## 🔒👤 **File Permissions**

* `chmod`: Change file permissions. Example: `chmod permissions filename`.
    
* `chown`: Change file owner. Example: `chown ownername filename`.
    
* `chgrp`: Change file group. Example: `chgrp groupname filename`.
    

## ⚙️🔄 **Processes**

* `ps`: Show the current processes.
    
* `top`: Monitor processes in real-time.
    
* `kill`: Terminate a process. Example: `kill process_id`.
    
* `killall`: Terminate all instances of a process. Example: `killall process_name`.
    
* `bg`: Move a process to the background.
    
* `fg`: Bring a background process to the foreground.
    
* `jobs`: List all background jobs.
    
* `nice`: Set the priority of a process. Example: `nice -n 10 command`.
    

## 🌐🔌 **Network**

* `ifconfig` or `ip`: Show network interface information.
    
* `ping`: Send ICMP echo requests to a host. Example: `ping` [`google.com`](http://google.com).
    
* `wget`: Download files from the web. Example: `wget URL`.
    
* `curl`: Transfer data with URLs. Example: `curl` [`https://www.example.com`](https://www.example.com).
    
* `netstat`: Show network statistics and active connections.
    
* `ss`: Show socket statistics.
    

## 🌳🔧 **Environment Variables**

* `env`: Show environment variables.
    
* `printenv`: Print environment variables.
    
* `export`: Set or modify an environment variable. Example: `export VAR=value`.
    
* `echo`: Print a message or the value of a variable. Example: `echo $VAR`.
    
* `source`: Read and execute commands from a file. Example: `source filename`.
    

## ✏️📝 **Text Editing with Vi**

* `vi`: Open the Vi text editor.
    
* `i`: To enter insert mode.
    
* `Esc`: To exit insert mode.
    
* `:wq`: To save and quit.
    
* `:q!`: To quit without saving.
    
* `dd`: Delete a line.
    
* `yy`: Copy (yank) a line.
    
* `p`: Paste the copied (yanked) line.
    
* `/pattern`: Search for a pattern in the file.
    
* `:%s/old/new/g`: Find and replace all occurrences of 'old' with 'new'.
    

## 👥🔑 **User Management**

* `who`: Show who is logged on.
    
* `whoami`: Show the current user.
    
* `useradd`: Add a new user. Example: `useradd username`.
    
* `passwd`: Set or change user password. Example: `passwd username`.
    
* `userdel`: Delete a user. Example: `userdel username`.
    
* `su`: Switch to another user. Example: `su - username`.
    
* `sudo`: Execute commands with superuser privileges. Example: `sudo command`.
    

## 🗜️📁 **File Compression**

* `tar`: Archive files. Example: `tar -cvf archive.tar file1 file2`.
    
* `gzip`: Compress files using gzip. Example: `gzip filename`.
    
* `gunzip`: Decompress files. Example: `gunzip filename.gz`.
    
* `zip`: Create a ZIP archive. Example: `zip` [`archive.zip`](http://archive.zip) `file1 file2`.
    
* `unzip`: Extract files from a ZIP archive. Example: `unzip` [`archive.zip`](http://archive.zip).
    
* `rar`: Create RAR archives. Example: `rar a archive.rar file1 file2`.
    
* `unrar`: Extract files from a RAR archive. Example: `unrar e archive.rar`.
    

## ℹ️🖥️ **System Information**

* `uname`: Show system information. Example: `uname -a`.
    
* `free`: Show memory usage.
    
* `df`: Display disk space usage.
    
* `du`: Show disk usage of files and directories.
    
* `uptime`: Show system uptime.
    
* `top`: Display real-time system status and resource usage.
    
* `ps`: Show process status.
    
* `lshw`: List hardware information.
    
* `lsblk`: List block devices.
    
* `history`: Show command history.
    

## 🌟 Conclusion

With this comprehensive cheat sheet at your disposal, you're equipped with a wide array of Linux commands to navigate through file systems, manage processes, configure networking, and handle user accounts. Embrace the power of Linux, experiment with these commands, and unveil the full potential of this open-source marvel. The mastery of these essentials will pave the way for a more productive and rewarding Linux journey. Happy command-line adventures! 🚀🌟