# 📘 Linux Command Reference Sheet

This repository provides a quick **cheat sheet of Linux commands** with simple explanations.  
Use it as a handy reference while working with the Linux terminal.

---

## 🔹 Getting Started with Linux

Linux is a family of open-source Unix-like operating systems. The terminal (or shell) is where most commands are executed.  
Common shells: **bash**, **zsh**, **fish**.

---

## 🖥️ Basic Commands

### `pwd`
Prints the **current working directory**.
```bash
pwd
```

### `ls`
Lists files and directories in the current folder.
```bash
ls       # list files
ls -l    # detailed list
ls -a    # include hidden files
```

### `cd`
Changes the current directory.
```bash
cd /home/user/Documents   # go to Documents
cd ..                     # go up one directory
```

### `clear`
Clears the terminal screen.

---

## 📂 File and Directory Management

### `touch`
Creates an empty file.
```bash
touch file.txt
```

### `mkdir`
Creates a new directory.
```bash
mkdir myfolder
```

### `cp`
Copies files or directories.
```bash
cp file.txt backup.txt
cp -r folder1 folder2   # copy directories recursively
```

### `mv`
Moves or renames files/directories.
```bash
mv oldname.txt newname.txt
mv file.txt /home/user/Desktop/
```

### `rm`
Removes files or directories.
```bash
rm file.txt
rm -r folder/   # remove directory recursively
```

---

## 📖 Viewing Files

### `cat`
Displays file content.
```bash
cat file.txt
```

### `less` / `more`
Views long files one page at a time.
```bash
less file.txt
more file.txt
```

### `head` / `tail`
Shows the beginning or end of a file.
```bash
head file.txt       # first 10 lines
tail file.txt       # last 10 lines
tail -f logfile.log # live monitor a log file
```
### `echo`
Show how to create and write to files.
```bash
echo "hello world!"> new.txt       # writes to the file
echo "hello world!">> new.txt      # appends to the file
```

------

## ⚙️ System Information

### `whoami`
Shows the current logged-in user.

### `uname`
Displays system information.
```bash
uname -a   # all system details
```

### `top`
Displays running processes and system usage.

### `df`
Shows disk usage.
```bash
df -h
```

### `free`
Displays memory usage.
```bash
free -m
```

---

## 🔎 Searching & Finding

### `find`
Searches for files/directories.
```bash
find /home -name "*.txt"
```

### `grep`
Searches inside files.
```bash
grep "error" logfile.txt
```

---

## 🌐 Networking

### `ping`
Checks connectivity to a host.
```bash
ping google.com
```

### `curl` / `wget`
Download content from the internet.
```bash
curl https://example.com
wget https://example.com/file.zip
```

### `ifconfig` / `ip`
Shows network configuration.
```bash
ip addr
```

---

## 🔑 User & Permissions

### `chmod`
Changes file permissions.
```bash
chmod 755 script.sh
```

### `chown`
Changes file ownership.
```bash
chown user:user file.txt
```

### `sudo`
Runs commands as superuser (administrator).
```bash
sudo apt update
```

---

## 📦 Package Management (Debian/Ubuntu)

### `apt`
Manages software packages.
```bash
sudo apt update       # update package list
sudo apt upgrade      # upgrade all packages
sudo apt install git  # install software
```

---

## 📚 Tips

- Use `man <command>` to read the manual of any command.
- Use `--help` with most commands for quick usage info.
```bash
man ls
ls --help
```

---

## ✅ Conclusion

This sheet provides a quick overview of **essential Linux commands**.  
For deeper learning, explore the manual pages or online documentation.
