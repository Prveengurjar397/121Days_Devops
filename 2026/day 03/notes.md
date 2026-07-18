# 📘 Day 03 Notes – Linux File Operations

## 🎯 Learning Objective

The goal of Day 03 is to learn how to create, copy, move, rename, delete, and search files and directories in Linux.

These commands are used daily by Linux Administrators and DevOps Engineers.

---

# 📂 What are File Operations?

File Operations are the basic tasks performed on files and directories.

Common operations include:

- Create
- Copy
- Move
- Rename
- Delete
- Search

---

# 📁 mkdir Command

The `mkdir` command is used to create a new directory.

### Syntax

```bash
mkdir directory_name
```

### Example

```bash
mkdir project
```

Create multiple directories:

```bash
mkdir backend frontend logs
```

Create nested directories:

```bash
mkdir -p project/backend/src
```


# 📄 touch Command

The `touch` command is used to create empty files.

### Syntax

```bash
touch filename
```

### Example

```bash
touch app.py
touch index.html
touch notes.txt
```

Create multiple files:

```bash
touch file1.txt file2.txt file3.txt
```


# 📋 cp Command

The `cp` command copies files or directories.

### Syntax

```bash
cp source destination
```

### Example

```bash
cp notes.txt backup.txt
```

Copy directory:

```bash
cp -r project backup_project
```


# 🚚 mv Command

The `mv` command moves or renames files.

### Rename Example

```bash
mv notes.txt linux-notes.txt
```

### Move Example

```bash
mv linux-notes.txt Documents/
```


# 🗑️ rm Command

The `rm` command removes files.

### Example

```bash
rm notes.txt
```

Delete directory:

```bash
rm -r project
```

Delete without confirmation:

```bash
rm -rf project
```

⚠️ **Be careful while using `rm -rf`.** It permanently deletes files and directories.


# 🔍 find Command

The `find` command searches for files and directories.

### Syntax

```bash
find location -name filename
```

### Example

```bash
find . -name "notes.txt"
```

Find Python files:

```bash
find . -name "*.py"
```


# 🔎 locate Command

The `locate` command searches files using a pre-built database.

### Example

```bash
locate notes.txt
```

If it doesn't work, update the database:

```bash
sudo updatedb
```


# 🌍 Real-World Example

Suppose your application log file is missing.

You can search it using:

```bash
find /var/log -name "*.log"
```

Or quickly locate it:

```bash
locate app.log
```

This helps DevOps Engineers troubleshoot systems efficiently.


# 🧪 Hands-on Practice

Practice these commands:

```bash
mkdir devops

cd devops

touch notes.txt

mkdir logs

cp notes.txt logs/

mv notes.txt linux-notes.txt

find . -name "linux-notes.txt"

locate linux-notes.txt

rm linux-notes.txt
```


# 📌 Key Takeaways

- `mkdir` → Create directories.
- `touch` → Create empty files.
- `cp` → Copy files/directories.
- `mv` → Move or rename files.
- `rm` → Delete files/directories.
- `find` → Search files in directories.
- `locate` → Quickly search files using a database.


# 🎯 Interview Questions

1. What is the purpose of the `mkdir` command?
2. What is the difference between `cp` and `mv`?
3. How do you rename a file in Linux?
4. What is the difference between `find` and `locate`?
5. Why should `rm -rf` be used carefully?
6. How do you copy an entire directory?
7. Which command creates an empty file?


# 📝 Student Assignment

✅ Create a folder named `devops-lab`.

✅ Create three files inside it.

✅ Copy one file to another folder.

✅ Rename a file.

✅ Delete one file.

✅ Search the remaining files using `find`.

✅ Commit today's work to GitHub.


# ✅ Revision Checklist

- [ ] Learn `mkdir`
- [ ] Learn `touch`
- [ ] Learn `cp`
- [ ] Learn `mv`
- [ ] Learn `rm`
- [ ] Learn `find`
- [ ] Learn `locate`
- [ ] Complete Hands-on Practice
- [ ] Revise Interview Questions


## 🏆 Today's Achievement

✅ Successfully completed **Day 03 – Linux File Operations**.

> "Mastering Linux file operations is the first step toward becoming confident in Linux administration and DevOps." 🚀
