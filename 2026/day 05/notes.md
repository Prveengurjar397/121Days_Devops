# 📘 Day 05 Notes – Linux User & Group Management

## 🎯 Learning Objective

The goal of Day 05 is to understand how Linux manages users and groups. Every DevOps Engineer must know how to create users, manage groups, assign permissions, and secure a Linux system.

---

# 👤 What is a User?

A **User** is an account that allows a person or service to log in and use the Linux system.

Every user has:
- Username
- User ID (UID)
- Home Directory
- Default Shell
- Password

Example:

```
praveen
ubuntu
root
```

---

# 👥 Types of Users

### 1. Root User

- UID = 0
- Has complete control over the system.
- Can perform all administrative tasks.

Command:

```bash
whoami
```

Output:

```
root
```

---

### 2. Normal User

- Created for daily work.
- Limited permissions.
- Cannot modify system files without sudo.

Example:

```
student
developer
```

---

### 3. System User

Used by Linux services and applications.

Examples:

```
mysql
nginx
www-data
```

These users generally cannot log in.

---

# 👥 What is a Group?

A **Group** is a collection of users.

Groups help manage permissions easily.

Instead of giving permissions to every user individually, we assign permissions to a group.

---

# 🔹 Check Current User

```bash
whoami
```

Example Output:

```
ubuntu
```

---

# 🔹 Check User ID

```bash
id
```

Example Output:

```
uid=1000(ubuntu)
gid=1000(ubuntu)
groups=1000(ubuntu)
```

---

# 🔹 Create a New User

```bash
sudo useradd devops
```

---

# 🔹 Set Password

```bash
sudo passwd devops
```

Linux will ask you to enter a new password.

---

# 🔹 Create a New Group

```bash
sudo groupadd developers
```

---

# 🔹 Add User to Group

```bash
sudo usermod -aG developers devops
```

Explanation:

- `-a` = Append
- `-G` = Secondary Group

---

# 🔹 Check User Groups

```bash
groups devops
```

Example:

```
devops : devops developers
```

---

# 🔹 Delete User

```bash
sudo userdel devops
```

Delete user along with home directory:

```bash
sudo userdel -r devops
```

---

# 🔹 Delete Group

```bash
sudo groupdel developers
```

---

# 📂 Important User Files

### `/etc/passwd`

Stores user account information.

View:

```bash
cat /etc/passwd
```

---

### `/etc/group`

Stores group information.

View:

```bash
cat /etc/group
```

---

# 🌍 Real-World Example

Suppose a company has three DevOps Engineers.

Instead of assigning permissions to each user separately:

```
Ravi
Aman
Priya
```

Create one group:

```
devops-team
```

Add all users:

```bash
sudo usermod -aG devops-team ravi
sudo usermod -aG devops-team aman
sudo usermod -aG devops-team priya
```

Now permission management becomes much easier.

---

# 🧪 Hands-on Practice

Practice these commands:

```bash
whoami

id

sudo useradd student1

sudo passwd student1

sudo groupadd devops

sudo usermod -aG devops student1

groups student1

cat /etc/passwd

cat /etc/group

sudo userdel -r student1

sudo groupdel devops
```

---

# 📌 Key Takeaways

- Every Linux account is called a User.
- Root User has complete control.
- Groups simplify permission management.
- `/etc/passwd` stores user information.
- `/etc/group` stores group information.
- `useradd` creates users.
- `groupadd` creates groups.
- `usermod -aG` adds users to groups.

---

# 🎯 Interview Questions

1. What is the difference between Root User and Normal User?
2. What is UID?
3. What is a Linux Group?
4. What is the purpose of `/etc/passwd`?
5. What is the purpose of `/etc/group`?
6. How do you create a user in Linux?
7. How do you add a user to a group?
8. What is the difference between `useradd` and `usermod`?

---

# 📝 Student Assignment

✅ Check your current user.

✅ Create a new user.

✅ Set a password.

✅ Create a new group.

✅ Add the user to the group.

✅ Verify group membership.

✅ Delete the test user and group.

✅ Commit today's work to GitHub.

---

# ✅ Revision Checklist

- [ ] Understand Linux Users
- [ ] Understand Linux Groups
- [ ] Practice `useradd`
- [ ] Practice `passwd`
- [ ] Practice `groupadd`
- [ ] Practice `usermod`
- [ ] Practice `userdel`
- [ ] Practice `groupdel`
- [ ] Explore `/etc/passwd`
- [ ] Explore `/etc/group`

---

## 🏆 Today's Achievement

✅ Successfully completed **Day 05 – Linux User & Group Management**.

> "Managing users and groups is one of the core responsibilities of every Linux Administrator and DevOps Engineer." 🚀
