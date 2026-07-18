# 📘 Day 06 Notes – Linux File Permissions & Ownership

## 🎯 Learning Objective

The goal of Day 06 is to understand Linux File Permissions and Ownership.

Every Linux file and directory has permissions that control who can read, write, and execute it. Proper permission management is essential for Linux Administrators and DevOps Engineers.

---

# 🔐 What are File Permissions?

File Permissions define who can:

- Read a file
- Modify a file
- Execute a file

Permissions help protect files from unauthorized access.

---

# 👥 Permission Categories

Linux divides permissions into three categories:

### User (u)

The owner of the file.

### Group (g)

Users who belong to the same group.

### Others (o)

All remaining users on the system.

---

# 📖 Permission Types

### Read (r)

Allows viewing the contents of a file.

Value:

```
4
```

---

### Write (w)

Allows modifying the file.

Value:

```
2
```

---

### Execute (x)

Allows running the file as a program or script.

Value:

```
1
```

---

# 🔍 View File Permissions

Command:

```bash
ls -l
```

Example:

```text
-rwxr-xr-- 1 ubuntu ubuntu 1200 Jul 18 script.sh
```

Explanation:

```
-        → File
rwx      → User
r-x      → Group
r--      → Others
```

---

# 🔢 Numeric Permissions

Permission values:

```
Read    = 4
Write   = 2
Execute = 1
```

Examples:

### 755

```
Owner  : rwx
Group  : r-x
Others : r-x
```

Command:

```bash
chmod 755 script.sh
```

---

### 644

```
Owner  : rw-
Group  : r--
Others : r--
```

Command:

```bash
chmod 644 notes.txt
```

---

### 777

```
Owner  : rwx
Group  : rwx
Others : rwx
```

Command:

```bash
chmod 777 file.txt
```

⚠️ Avoid using **777** on production servers because it allows everyone full access.

---

# ✍️ Symbolic Permissions

Add Execute Permission:

```bash
chmod +x script.sh
```

Remove Write Permission:

```bash
chmod -w notes.txt
```

Give Read Permission to Group:

```bash
chmod g+r notes.txt
```

---

# 👤 Change File Ownership

Command:

```bash
sudo chown user file.txt
```

Example:

```bash
sudo chown devops notes.txt
```

---

# 👥 Change Owner and Group

```bash
sudo chown devops:developers notes.txt
```

---

# 🌍 Real-World Example

Suppose a deployment script should only be executed by the owner.

Set permission:

```bash
chmod 700 deploy.sh
```

Only the owner can:

- Read
- Write
- Execute

Other users cannot access the file.

---

# 🧪 Hands-on Practice

Practice these commands:

```bash
touch notes.txt

ls -l

chmod 644 notes.txt

chmod +x notes.txt

chmod 755 notes.txt

sudo chown $USER notes.txt

ls -l
```

---

# 📌 Key Takeaways

- Linux permissions improve system security.
- Every file has an owner and a group.
- `chmod` changes permissions.
- `chown` changes ownership.
- 755 is commonly used for executable files.
- 644 is commonly used for normal files.
- Avoid using 777 unless absolutely necessary.

---

# 🎯 Interview Questions

1. What are Linux File Permissions?
2. What do Read, Write, and Execute mean?
3. What is the difference between 755 and 644?
4. What is the purpose of chmod?
5. What is the purpose of chown?
6. Why should 777 be avoided?
7. What is the difference between symbolic and numeric permissions?

---

# 📝 Student Assignment

✅ Create a file named `practice.txt`.

✅ Check its permissions using `ls -l`.

✅ Change permission to **644**.

✅ Change permission to **755**.

✅ Add execute permission using symbolic mode.

✅ Change file ownership.

✅ Verify the changes using `ls -l`.

✅ Commit today's work to GitHub.

---

# ✅ Revision Checklist

- [ ] Understand Linux Permissions
- [ ] Learn Read, Write, Execute
- [ ] Practice `ls -l`
- [ ] Practice `chmod`
- [ ] Practice `chown`
- [ ] Understand 755
- [ ] Understand 644
- [ ] Complete Hands-on Practice
- [ ] Revise Interview Questions

---

## 🏆 Today's Achievement

✅ Successfully completed **Day 06 – Linux File Permissions & Ownership**.

> "Understanding Linux permissions is essential for securing servers and becoming a skilled DevOps Engineer." 🚀
