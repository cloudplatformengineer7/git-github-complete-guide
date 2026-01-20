# Git Installation and Configuration

This document explains how to **install Git** on different operating systems and perform the **basic configuration** required before using Git.

---

## 1. Install Git

### Windows

1. Download Git from: https://git-scm.com/download/win  
2. Run the installer and follow the default setup  
3. Open **Git Bash** after installation

---

### macOS

Using Homebrew:

brew install git

Or download from: https://git-scm.com/download/mac


Linux:

Ubuntu / Debian:

sudo apt update
sudo apt install git

CentOS / RHEL:

sudo yum install git

###Verify Installation

Check if Git is installed successfully:

git --version

Expected output:

git version 2.x.x

### Configure Git User Details

Git requires a username and email address to identify commit authors.

git config --global user.name "Your Name"
git config --global user.email "your@email.com"

### Verify Configuration

View all configured settings:

git config --list


### Optional Configuration

Set Default Branch Name

git config --global init.defaultBranch main

Set Default Editor (VS Code)

git config --global core.editor "code --wait"

