# Linux and Unix Fundamentals

<p align="center">
  <img src="https://user-images.githubusercontent.com/74038190/212259380-f2671dad-3359-4b3b-96e7-2f011c844a84.jpg" width="350" />
</p>

  <p align="center">Welcome to the Linux and Unix fundamentals section!</p>


## Table of Contents

1. [Introduction](#introduction)
2. [File System](#file-system)
3. [Command Line Basics](#command-line-basics)
4. [Permissions](#permissions)
5. [Processes](#processes)
6. [Package Management](#package-management)
7. [Shell Scripting](#shell-scripting)
8. [Networking](#networking)
9. [System Administration](#system-administration)

## Introduction

Linux and Unix are powerful, open-source operating systems that form the backbone of many computing environments. Understanding their fundamentals is crucial for efficient and effective system administration and development.

## File System

### Directory Structure

The file system in Linux and Unix is hierarchical. Key directories include:
- `/`: The root directory
- `/home`: Home directories for users
- `/etc`: Configuration files
- `/bin` and `/usr/bin`: Executable binaries
- `/var`: Variable data (logs, temporary files)

### Basic Commands

- `ls`: List files and directories
- `cd`: Change directory
- `cp`, `mv`, `rm`: Copy, move, and remove files
- `mkdir`, `rmdir`: Create and remove directories
- `cat`, `less`: Display file contents

## Command Line Basics

The command line is a powerful interface to interact with the system. Here are some essential commands:

- `pwd`: Print current working directory
- `echo`: Display text
- `man`: Display manual pages for commands
- `grep`: Search for patterns in files
- `ps`: Display information about processes
- `kill`: Terminate processes

## Permissions

Linux and Unix use a robust permissions system. Key commands include:

- `chmod`: Change file permissions
- `chown`: Change file owner
- `chgrp`: Change file group

## Processes

Understanding processes is vital for system management. Key commands include:

- `ps`: Display information about processes
- `top`: Display real-time system statistics
- `kill`: Terminate processes

## Package Management

Package managers simplify software installation and management. Common package managers are `apt` (Debian/Ubuntu), `yum` (Red Hat), and `pacman` (Arch). Use commands like `apt-get`, `yum install`, and `pacman -S` to install packages.

## Shell Scripting

Shell scripting automates tasks. Learn to create and execute shell scripts using tools like `bash`. Understand variables, loops, and conditionals.

## Networking

Linux and Unix excel in networking. Key commands include:

- `ifconfig` or `ip`: Configure network interfaces
- `ping`: Test network connectivity
- `netstat` or `ss`: Display network statistics

## System Administration

System administration involves configuring and managing the system. Key tasks include:

- User management: `useradd`, `passwd`, `userdel`
- System updates: `apt update`, `yum update`
- System logs: Check `/var/log` for system logs

## File System

### Tip 1: Understand the File Hierarchy

Familiarize yourself with the Linux file system hierarchy. Key directories like `/`, `/home`, `/etc`, and `/var` play crucial roles. Knowing their purposes will make navigation easier.

```bash
cd /     # Navigate to the root directory
cd ~     # Shortcut to your home directory
```
### Tip 2: Master Basic File Operations

Learn fundamental file operations to navigate and manipulate files.

```bash
ls         # List files and directories
cp, mv, rm # Copy, move, and remove files
mkdir      # Create a new directory
```

## Command line basics 
### Tip 3: Leverage Tab Completion

Save time by using tab completion. Start typing a command or file path, then press Tab to autocomplete or display options.

```bash
cd /ho[TAB]  # Autocomplete to cd /home/
```
### Tip 4: Explore the 'man' Pages

Use the man command to access manual pages for commands. It provides in-depth information on command usage and options.

```bash
man ls  # Display manual for the 'ls' command
```
## Permisissons 
### Tip 5: Understand File Permissions

Master the chmod, chown, and chgrp commands to manage file permissions. Understanding the symbolic representation (e.g., rwxr-xr--) is essential.

```bash
chmod 755 file  # Give read, write, and execute permissions to the owner, and read and execute permissions to others
```
### Tip 6: Use 'sudo' Wisely

Be cautious when using the sudo command to execute commands with elevated privileges. It is a powerful tool, so use it only when necessary.

```bash
sudo apt update  # Update package lists with elevated privileges
```
## Processes 
### Tip 7: Monitor System Processes

Use tools like ps and top to monitor running processes and system resource usage.

```bash
ps aux  # Display detailed information about all running processes
top     # Display real-time system statistics

```
### Tip 8: Safely Terminate Processes
When needed, terminate processes using the kill command. Use kill -9 for forceful termination.
```bash
kill PID  # Terminate a process by its ID
```
## Package Management 
### Tip 9: Keep Software Updated
Regularly update your system and installed software packages to ensure security and stability.
```bash
sudo apt update       # Update package lists
sudo apt upgrade      # Upgrade installed packages
```
### Tip 10: Explore Package Managers
Different distributions use different package managers (e.g., apt, yum, pacman). Familiarize yourself with the package manager relevant to your distribution.
```bash
sudo apt install package_name  # Install a package using 'apt'
```
## Shell Scripting
### Tip 11: Start with Basic Shell Scripts
Experiment with simple shell scripts to automate repetitive tasks. Learn about variables, loops, and conditionals.
```bash
#!/bin/bash
echo "Hello, world!"
```
## Networking
### Tip 12: Use Network Commands
Explore commands like ifconfig or ip, ping, and netstat to troubleshoot and manage network configurations.
```bash
ifconfig      # Display network interface information
ping google.com  # Test network connectivity
netstat -an   # Display all active network connections
```
## System Administration
### Tip 13: Learn Basic System Administration
Become familiar with basic system administration tasks, such as user management, system updates, and monitoring logs.
```bash
sudo useradd username  # Add a new user
sudo apt upgrade        # Upgrade installed packages
cat /var/log/syslog     # Display system logs
```
## Backup and Restore
### Tip 14: Backup Regularly
Back up your important files and configurations regularly. Consider tools like rsync or dedicated backup solutions.
```bash
rsync -av source/ destination/  # Sync files from source to destination
```
### Tip 15: Embrace Community Resources
Join Linux and Unix forums, communities, and online tutorials. The open-source community is vast and supportive.

# LINUX - UNIX CHARTS

### _File Management_
| Command | Description                              |
| ------- | ---------------------------------------- |
| `du`    | Decipher disk usage for files and directories. |
| `df`    | Delve into filesystem disk space usage.   |
| `fdisk` | Fashion disk partitions with precision.   |

### _Data Exploration and Manipulation_
| Command         | Description                                      |
| --------------- | ------------------------------------------------ |
| `sort`          | Streamline content into sorted order.             |
| `grep`, `egrep`, `fgrep` | Gracefully extract patterns within text. |
| `sed`           | Seamlessly edit streams of data.                 |
| `awk`           | Agilely process text with pattern scanning and processing. |

### _File Compression and Archiving_
| Command              | Description                                      |
| -------------------- | ------------------------------------------------ |
| `gzip`, `gzcat`, `gunzip` | Gracefully zip and unzip files.                  |
| `tar`                | Tie files together effortlessly.                 |
| `zip`, `unzip`       | Zip and unzip files with ease.                   |
| `bzip2`              | Boldly compress files for compact storage.       |

### _Environment and Shell Customization_
| Command               | Description                                      |
| --------------------- | ------------------------------------------------ |
| `printenv`, `env`, `set` | Probe environment variables with clarity.       |
| Bash Default Variants | Bend the bash shell to your will.                 |
| `umask`               | Unmask default file permissions.                  |
| `fsck`                | Faithfully check and repair filesystems.          |

