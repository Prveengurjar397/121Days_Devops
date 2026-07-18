# 📘 Day 04 Notes – Linux Text Editors (Vim & Nano)

## 🎯 Learning Objective

The goal of Day 04 is to learn how to create, edit, save, and manage files using the Nano and Vim text editors.

Text editors are one of the most frequently used tools by Linux Administrators and DevOps Engineers because almost every configuration file, script, Dockerfile, Kubernetes manifest, and Ansible Playbook is edited using a terminal-based editor.

---

# 📝 What is a Text Editor?

A Text Editor is a software application used to create and edit plain text files.

Linux provides many text editors, but the most commonly used are:

- Nano
- Vim
- Vi

---

# 📌 Nano Editor

Nano is a simple and beginner-friendly text editor.

It is easy to use because shortcut keys are displayed at the bottom of the screen.

### Open or Create a File

```bash
nano notes.txt
```

If the file does not exist, Nano creates it automatically.

---

## Basic Nano Shortcuts

| Shortcut | Description |
|----------|-------------|
| Ctrl + O | Save File |
| Enter | Confirm Save |
| Ctrl + X | Exit Nano |
| Ctrl + K | Cut Current Line |
| Ctrl + U | Paste Line |
| Ctrl + W | Search Text |

---

## Example

```bash
nano devops.txt
```

Write:

```
Welcome to Linux
Learning DevOps
```

Save:

```
Ctrl + O
Enter
```

Exit:

```
Ctrl + X
```

---

# 📌 Vim Editor

Vim (Vi Improved) is a powerful terminal-based text editor.

Unlike Nano, Vim works in different modes.

---

## Vim Modes

### 1. Normal Mode

Default mode.

Used for:

- Navigation
- Copy
- Delete
- Paste

---

### 2. Insert Mode

Used to type text.

Press:

```
i
```

to enter Insert Mode.

---

### 3. Command Mode

Used for saving and quitting.

Press:

```
Esc
```

then type commands.

---

## Open or Create a File

```bash
vim notes.txt
```

---

## Save and Exit

Save:

```
:w
```

Save and Exit:

```
:wq
```

Exit without Saving:

```
:q!
```

---

## Basic Vim Commands

| Command | Description |
|----------|-------------|
| i | Insert Mode |
| Esc | Return to Normal Mode |
| :w | Save File |
| :q | Quit |
| :wq | Save & Quit |
| :q! | Quit without Saving |
| dd | Delete Current Line |
| yy | Copy Current Line |
| p | Paste |

---

# 🌍 Real-World Example

A DevOps Engineer may edit:

- `/etc/nginx/nginx.conf`
- Dockerfile
- `docker-compose.yml`
- Kubernetes YAML files
- Jenkinsfile
- Ansible Playbooks

These files are usually edited using **Vim** or **Nano** directly on Linux servers.

---

# 🧪 Hands-on Practice

Practice the following commands:

```bash
nano notes.txt
```

Write some text.

Save and Exit.

Now open the same file:

```bash
vim notes.txt
```

Enter Insert Mode:

```
i
```

Edit the file.

Press:

```
Esc
```

Save and Exit:

```
:wq
```

---

# 📌 Key Takeaways

- Nano is beginner-friendly.
- Vim is powerful and widely used.
- Vim has Normal, Insert, and Command modes.
- Most Linux configuration files are edited using Vim.
- Learning Vim is essential for every DevOps Engineer.

---

# 🎯 Interview Questions

1. What is Nano Editor?
2. What is Vim Editor?
3. What is the difference between Nano and Vim?
4. What are the different modes in Vim?
5. How do you save and quit a file in Vim?
6. How do you quit Vim without saving changes?
7. Why do DevOps Engineers use Vim?

---

# 📝 Student Assignment

✅ Create a file using Nano.

✅ Edit the same file using Vim.

✅ Practice saving and exiting both editors.

✅ Write today's learning in your own words.

✅ Commit today's work to GitHub.

---

# ✅ Revision Checklist

- [ ] Understand Nano Editor
- [ ] Learn Nano Shortcuts
- [ ] Understand Vim Modes
- [ ] Practice Basic Vim Commands
- [ ] Complete Hands-on Practice
- [ ] Revise Interview Questions


## 🏆 Today's Achievement

✅ Successfully completed **Day 04 – Linux Text Editors (Vim & Nano).**

> "The better you master Vim, the faster you work as a Linux Administrator and DevOps Engineer." 🚀
