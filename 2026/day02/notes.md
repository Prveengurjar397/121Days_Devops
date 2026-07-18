# 📘 Day 02 Notes – Linux Directory Structure & Important System Paths

## 🎯 Learning Objective

The goal of Day 02 is to understand the Linux File System Hierarchy (FHS) and learn the purpose of important system directories used by Linux and DevOps Engineers.


# 📂 What is Linux File System Hierarchy (FHS)?

The Linux File System Hierarchy (FHS) is a standard structure that defines where files and directories are stored in a Linux operating system.

Unlike Windows, Linux starts from a single root directory called `/`.

```
        /
       ├── bin
       ├── boot
       ├── dev
       ├── etc
       ├── home
       ├── lib
       ├── media
       ├── mnt
       ├── opt
       ├── proc
       ├── root
       ├── run
       ├── sbin
       ├── srv
       ├── sys
       ├── tmp
       ├── usr
       └── var
```

---

# 📁 Important Linux Directories

## 1️⃣ `/`

This is the **Root Directory**.

- It is the top-level directory.
- Every file and folder starts from `/`.

Example:

```bash
cd /
```

---

## 2️⃣ `/home`

Stores personal files of normal users.

Example:

```
/home/praveen
/home/student
```

---

## 3️⃣ `/root`

Home directory of the **root (administrator)** user.

Only the root user has full access.

---

## 4️⃣ `/etc`

Stores system configuration files.

Examples:

- passwd
- hosts
- ssh configuration
- network configuration

DevOps engineers frequently work inside this directory.

---

## 5️⃣ `/var`

Stores variable data.

Examples:

- System logs
- Cache
- Mail
- Application logs

Important path:

```
/var/log
```

---

## 6️⃣ `/usr`

Stores user applications and utilities.

Examples:

- Programs
- Libraries
- Documentation

---

## 7️⃣ `/bin`

Contains essential Linux commands.

Examples:

```bash
ls
cp
mv
cat
pwd
echo
```


## 8️⃣ `/sbin`

Contains system administration commands.

Examples:

- reboot
- shutdown
- fsck

Mostly used by the root user.

---

## 9️⃣ `/opt`

Used for optional or third-party software.

Example:

```
/opt/google
/opt/docker
```


## 🔟 `/tmp`

Stores temporary files.

Files may be deleted automatically after reboot.


## 1️⃣1️⃣ `/dev`

Contains device files.

Examples:

- Hard Disk
- USB
- Keyboard
- Mouse

Linux treats devices as files.


## 1️⃣2️⃣ `/proc`

A virtual file system.

Provides information about:

- CPU
- Memory
- Running Processes

Useful for troubleshooting.


## 🌍 Real-World Example

Suppose an application is not working.

A DevOps Engineer may check:

```
/var/log
```

to read logs,

or

```
/etc
```

to verify configuration files.

Understanding these directories helps solve issues faster.


# 🧪 Hands-on Practice

Practice these commands:

```bash
pwd
cd /
ls
cd /home
cd /etc
cd /var
cd /tmp
cd /usr
cd /opt
```

Explore each directory using:

```bash
ls
```

---

# 📌 Key Takeaways

- Linux starts from the Root Directory (`/`).
- `/etc` stores configuration files.
- `/var` stores logs and changing data.
- `/home` stores user files.
- `/root` is the root user's home directory.
- `/tmp` stores temporary files.
- `/proc` provides system information.
- `/dev` contains device files.


# 🎯 Interview Questions

1. What is the Linux File System Hierarchy?
2. What is the purpose of the `/etc` directory?
3. What is stored inside `/var`?
4. What is the difference between `/home` and `/root`?
5. Why is `/tmp` used?
6. What is `/proc`?
7. Why is `/dev` important?


# 📝 Student Assignment

✅ Navigate through all important directories.

✅ Write the purpose of each directory in your own words.

✅ Explore `/var/log`.

✅ Explore `/etc`.

✅ Commit today's work to GitHub.


# ✅ Revision Checklist

- [ ] Understand Linux File System Hierarchy
- [ ] Learn Root Directory
- [ ] Learn `/etc`
- [ ] Learn `/var`
- [ ] Learn `/home`
- [ ] Learn `/root`
- [ ] Learn `/usr`
- [ ] Learn `/tmp`
- [ ] Revise Interview Questions


## 🏆 Today's Achievement

✅ Successfully completed **Day 02 – Linux Directory Structure & Important System Paths**.

> "Understanding the Linux File System is the foundation of Linux Administration and DevOps." 🚀
