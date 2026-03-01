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

# 🚀 Steps to Start Practice Course with PathNex

This guide will help you:

* Create one GitHub repository
* Organize daily practice files
* Push your work to GitHub
* Maintain a proper daily routine

---

# ✅ PART 1 — Create One GitHub Repository

1. Go to [https://github.com](https://github.com)
2. Login to your account
3. Click **+ (top right)** → **New repository**
4. Repository name:

   ```
   Batch_Name_Pathnex
   Example: Dec2025_Neeraj_Pathnex
   ```
5. Select **Public**
6. Do NOT add README (optional)
7. Click **Create repository**

✅ Your GitHub repository is ready.

---

# ✅ PART 2 — Prepare Local Project (On Your Laptop)

Open **Terminal / Git Bash** and follow the steps below.

---

## 🔹 Step 1 — Create Project Folder

```bash
mkdir Batch_Name_Pathnex
cd Batch_Name_Pathnex
```

---

## 🔹 Step 2 — Create Two Folders

```bash
mkdir timings
mkdir "coding practice"
```

---

## 🔹 Step 3 — Create Today’s Files

Example file name:

```
Day01-06-Dec-2025.txt
```

Create files inside both folders:

```bash
# Inside timings
vim timings/Day01-06-Dec-2025.txt

# Inside coding practice
vim "coding practice/Day01-06-Dec-2025.txt"
```

Add your content and save the files.

---

## 📂 Folder Structure

```
Batch_Name_Pathnex/
├── timings/
│     └── Day01-06-Dec-2025.txt
└── coding practice/
      └── Day01-06-Dec-2025.txt
```

---

# 📝 Sample — timings File Format

```
----------------------------------------

What I did today:
- 1 hour - Revised Datadog
- 30 mins coding
- 1 hour English speaking / watching movies
- 2 hours - Question practice

Tomorrow's Task:
- ELK, Kafka, Terraform revision
- 1 hour coding
- 1 hour English reading
- 1 hour Question paper practice

----------------------------------------
```

---

# ✅ PART 3 — Push to GitHub from Local

---

## 🔹 Step 1 — Initialize Git

```bash
git init
```

---

## 🔹 Step 2 — Add Remote Repository

Copy your GitHub repository HTTPS URL and run:

```bash
git remote add origin https://github.com/your-username/Batch_Name_Pathnex.git
```

---

## 🔹 Step 3 — Add All Files

```bash
git add .
```

---

## 🔹 Step 4 — Commit

```bash
git commit -m "Added Day01 files in timings and coding practice"
```

---

## 🔹 Step 5 — Push to GitHub

```bash
git branch -M main
git push -u origin main
```

🎉 Congratulations! Your files are now uploaded to GitHub.

---

# 🔄 Daily Routine (From Next Day)

1. Create new files for the new day
   Example:

   ```
   Day02-07-Dec-2025.txt
   ```

2. Add files inside both folders.

3. Then run:

```bash
git add .
git commit -m "Added Day02 files"
git push
```

---

# 📌 Final Repository Structure

```
Batch_Name_Pathnex/
├── timings/
│     ├── Day01-06-Dec-2025.txt
│     ├── Day02-07-Dec-2025.txt
│     └── ...
└── coding practice/
      ├── Day01-06-Dec-2025.txt
      ├── Day02-07-Dec-2025.txt
      └── ...
```

---

# ⭐ Best Practice (Recommended)

For better Git workflow:

* Create a new branch daily
* Make changes
* Commit changes
* Push branch
* Create Pull Request (PR)
* Merge into main
* Delete old branch

Example:

```bash
git checkout -b day02-update
git add .
git commit -m "Added Day02 files"
git push origin day02-update
```

Then create PR on GitHub and merge.

---

# ✅ Summary

✔ One GitHub Repository
✔ Daily Practice Tracking
✔ Proper Folder Structure
✔ Git Version Control
✔ Professional Workflow


