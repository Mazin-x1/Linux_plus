# Linux Fundamentals  
### System Usage, Commands, and Security Basics  

---

## 📌 Overview
This module covers the fundamentals of Linux systems, including installation methods, command-line usage, file management, permissions, and basic system operations.

It demonstrates practical understanding of:
- Linux environments
- Terminal usage
- File system navigation
- Permissions and security
- Basic system monitoring

---

## 🧠 What is Linux?

Linux is an **open-source operating system** that allows users to:
- Modify source code
- Customize system behavior
- Use powerful command-line tools

### Key Characteristics
- Open-source and customizable  
- More secure (permission-based system)  
- Widely used in servers, cybersecurity, and Android systems  

---

## 🐧 Linux Distributions

Common distributions:
- Debian (Kali Linux)
- Ubuntu
- Red Hat
- Fedora
- CentOS  

> Each distribution serves different use cases (security, servers, desktop).

---

## 💻 Installation Methods

### 1️⃣ Primary Installation
- Linux is installed as the main OS  
- Device boots directly into Linux  

### 2️⃣ Virtual Machine
- Run Linux inside tools like VMware  
- Safe for testing and learning  

### 3️⃣ Bootable USB
- Run Linux without installing  
- Useful for forensics or temporary usage  

---

## 🔄 System Update

```bash
sudo apt update
sudo apt upgrade
````

* `sudo` → run as root (high privileges)
* `apt` → package manager

---

## 🧑‍💻 User Management

```bash
sudo su
exit
whoami
```

* Switch to root user
* Return to normal user
* Check current user

---

## 📁 File System Navigation

```bash
ls
pwd
cd folder_name
cd ..
```

* List files
* Show current directory
* Navigate folders

---

## 📄 File Operations

```bash
cat file.txt
nano file.txt
rm file.txt
mkdir folder
rm -r folder
```

* Read files
* Create/edit files
* Delete files/folders

---

## 📂 File Movement

```bash
mv file.txt /home
mv file.txt newname.txt
cp file.txt /home
```

* Move / rename files
* Copy files

---

## ✍️ Writing vs Appending

```bash
echo "text" > file.txt
echo "text" >> file.txt
```

* `>` overwrite
* `>>` append

---

## 📊 System Information

```bash
ifconfig
free
df -H
ps aux
```

* Network info
* Memory usage
* Disk usage
* Running processes

---

## 📦 Installing Applications

```bash
apt install app
snap install app
dpkg -i file.deb
```

* Different installation methods

---

## 🔐 Linux Permissions

### Permission Types

* Read (r) = 4
* Write (w) = 2
* Execute (x) = 1

### Examples

* 7 = rwx
* 6 = rw-
* 3 = -wx

```bash
ls -lah
chmod 777 file.txt
chmod +x file.txt
```

### Permission Structure

* Owner
* Group
* Others

---

## 🧠 Paths

* **Absolute Path:** `/home/user/file`
* **Relative Path:** based on current location

---

## 🔗 Piping & Redirection

```bash
cat file.txt | grep "text"
cat file.txt | wc
```

* `|` sends output to another command

---
## ⚠️ Security Awareness

* Root access can destroy system if misused
* Always be careful when using:

```bash
sudo rm -r
```

* Stop running process:

```bash
Ctrl + C
```

* Clear terminal:

```bash
clear
```

---

## 🛡️ Security Insight

Linux security relies heavily on:

* Proper permissions
* User privilege separation
* Secure command usage

Most attacks happen due to:
❌ Misconfigured permissions
❌ Running commands as root without caution

---

## 🙌 Conclusion

Linux is a core skill in cybersecurity, enabling full control over systems, tools, and network interactions.
