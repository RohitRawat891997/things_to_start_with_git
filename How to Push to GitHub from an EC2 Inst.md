## 🌐 Connect With Me

<p align="center">
  <a href="mailto:rohitrawat89199@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-FF6B6B?style=for-the-badge&logo=gmail&logoColor=white&labelColor=00000020" />
  </a>
  <a href="https://www.linkedin.com/in/rohit-rawat-7383091a7/">
    <img src="https://img.shields.io/badge/LinkedIn-58A6FF?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=00000020" />
  </a>
  <a href="https://github.com/RohitRawat891997">
    <img src="https://img.shields.io/badge/GitHub-1F2328?style=for-the-badge&logo=github&logoColor=white&labelColor=00000020" />
  </a>
  <a href="https://hub.docker.com/u/rohitrawat891997">
    <img src="https://img.shields.io/badge/DockerHub-2496ED?style=for-the-badge&logo=docker&logoColor=white&labelColor=00000020" />
  </a>
</p>

---

# 🚀 Push Code to GitHub from an EC2 Instance (Step-by-Step Guide)

This guide explains how to push code to GitHub from an AWS EC2 instance.

---

## ✅ Step 1 — Install Git on EC2

### 🔹 Amazon Linux / RHEL / CentOS

```bash
sudo yum install git -y
```

### 🔹 Ubuntu

```bash
sudo apt update
sudo apt install git -y
```

---

## ✅ Step 2 — Configure Git (One-Time Setup)

Set your Git username and email (run once):

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Verify configuration:

```bash
git config --list
```

---

## ✅ Step 3 — Authenticate to GitHub

You can authenticate using **SSH (Recommended)** or **HTTPS + Personal Access Token**.

---

# 🔐 Option A — SSH Key Method (Recommended)

### 1️⃣ Generate SSH Key on EC2

```bash
ssh-keygen -t ed25519 -C "your@email.com"
```

Press **Enter** for all prompts.

Your keys will be saved at:

```
~/.ssh/id_ed25519
~/.ssh/id_ed25519.pub
```

---

### 2️⃣ Copy Public Key

```bash
cat ~/.ssh/id_ed25519.pub
```

Copy the entire output.

---

### 3️⃣ Add SSH Key to GitHub

1. Go to GitHub → Profile → **Settings**
2. Click **SSH and GPG keys**
3. Click **New SSH Key**
4. Paste the key
5. Click **Save**

---

### 4️⃣ Test SSH Connection

```bash
ssh -T git@github.com
```

If successful, you will see:

```
Hi username! You've successfully authenticated.
```

✅ You are now ready to push code.

---

# 🔑 Option B — HTTPS + Personal Access Token (PAT)

If using HTTPS, GitHub does **not** accept passwords.

### Generate Personal Access Token:

1. GitHub → Settings
2. Developer Settings
3. Personal Access Tokens
4. Generate new token
5. Select required permissions (repo)
6. Generate and copy the token

Use this token instead of your password when pushing.

---

## ✅ Step 4 — Clone Your Repository on EC2

### Using SSH (Recommended)

```bash
git clone git@github.com:yourusername/yourrepo.git
```

Move into the directory:

```bash
cd yourrepo
```

---

## ✅ Step 5 — Make Changes and Commit

Example:

```bash
echo "Hello from EC2" > hello.txt

git add .
git commit -m "Added hello.txt from EC2"
```

---

## ✅ Step 6 — Push to GitHub

```bash
git push
```

🎉 Your code is now successfully pushed from EC2 to GitHub!

---

# 🔎 Quick Workflow Summary

```bash
git clone <repo>
cd <repo>
# make changes
git add .
git commit -m "message"
git push
```
