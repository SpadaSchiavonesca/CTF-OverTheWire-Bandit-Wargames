# 🛡️ OverTheWire Bandit CTF - Level 0: SSH Connection Success 🚀

## Demonstrating Foundational Cybersecurity Skills

This document outlines my successful completion of **Bandit Level 0** from the OverTheWire Capture The Flag (CTF) challenges. OverTheWire Bandit is a fantastic resource for learning essential cybersecurity and Linux command-line skills in a gamified environment.  This level focused on establishing a fundamental skill for any cybersecurity professional: **connecting to remote servers securely via SSH.**

---

## Challenge Overview: OverTheWire Bandit 🚩

**OverTheWire Bandit** provides a series of progressively challenging levels that teach Linux command-line expertise and core cybersecurity concepts. Starting from Level 0, the challenges are designed to be beginner-friendly and gradually introduce more complex topics.

**Level 0 Objective:**  Establish a secure SSH connection to the Bandit game server.

---

## ✅ Steps to Successful SSH Connection

Here are the steps I took to successfully complete Bandit Level 0:

1.  **Open a Terminal:** Accessed the command-line interface on my local machine (essential for interacting with remote servers).

2.  **Execute the SSH Command:**  Utilized the `ssh` command, the standard tool for secure remote connections, with the specific parameters provided by OverTheWire:

    ```bash
    ssh bandit0@bandit.labs.overthewire.org -p 2220
    ```
    *(This command instructs SSH to connect to the username `bandit0` at the server address `bandit.labs.overthewire.org` using port `2220`.)*

3.  **Acknowledge Host Key (First Connection):**  Upon the initial connection, securely acknowledged and added the server's host key to my known hosts file, ensuring future connections are verified.

4.  **Successful Connection Established:**  Confirmed successful SSH connection upon receiving the server's welcome message (motd).

---

## 💻 Expected Terminal Output (Confirmation of Success)

The following terminal output clearly indicates a successful SSH connection to the Bandit server:

```text
The authenticity of host '[bandit.labs.overthewire.org]:2220 ([bandit.labs.overthewire.org]:2220)' can't be established.
ECDSA key fingerprint is SHA256:C6CBtOx06GxsVjQ/kY6sXeR8/ST+9r4j9cQWPAo0d2w.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[bandit.labs.overthewire.org]:2220' (ECDSA) to the list of known hosts.
