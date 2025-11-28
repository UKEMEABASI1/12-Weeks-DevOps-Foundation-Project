# ✅ **Week 1 Git Activities — with Commands**

---

## **1. Install Git**

### **Ubuntu / Debian**

```bash
sudo apt update
sudo apt install git -y
```

### **Windows Chocolatey (if you have choco installed)

```
choco install git -y
```

Confirm:

```
git --version
```

---

## **2. Configure Global Username & Email**

These details will attach your identity to every commit.

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

To verify:

```bash
git config --global --list
```

---

## **3. Generate SSH Keys**

Generates a secure key for GitHub authentication.

```bash
ssh-keygen -t ed25519 -C "your-email@example.com"
```

When asked for file location, just press **ENTER** to accept default:

```
/home/youruser/.ssh/id_ed25519
```

Start ssh-agent:

```bash
eval "$(ssh-agent -s)"
```

Add your private key:

```bash
ssh-add ~/.ssh/id_ed25519
```

---

## **4. Add SSH Key to GitHub**

Copy the public key:

```bash
cat ~/.ssh/id_ed25519.pub
```

Copy the output → go to **GitHub → Settings → SSH and GPG Keys → New SSH Key** → paste → Save.

Test connection:

```bash
ssh -T git@github.com
```

Expected message:

```
Hi <username>! You've successfully authenticated...
```

---

## **5. Create Your First Git Repo**

### **Initialize a local repository**

```bash
mkdir my-demo-repo
cd my-demo-repo
git init
```

### **Create a README file**

```bash
echo "# My demo Repo" > README.md (optional could also be done on the github console)
```

---

## **6. Make Your First Commit**

```bash
git add .
git commit -m "Initial commit: Added Team-Ai" 
```

---

## **7. Create a GitHub Repo (manual step)**

Go to GitHub → **New Repository**
Name: `my-demo-repo`
Do **NOT** initialize README (if you already have one I did no create a readme for my-Demo-repo).

Copy your repo’s SSH link: https://github.com/Your Username/your-repo-name.git

```
git@github.com:UKEMEABASI1/my-demo-repo.git
```

---

## **8. Add Remote & Push to GitHub**

```bash
git remote add origin git@github.com:UKEMEABASI1/my-demo-repo.git
git branch -M main
git push -u origin main
```
## **9. Go to Github and create a Pull request 
