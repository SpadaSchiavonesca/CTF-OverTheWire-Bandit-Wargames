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

3.  **Acknowledge Host Key (First Connection - if prompted):**  Upon the initial connection, you might be prompted to acknowledge and add the server's host key.  In this case, for Bandit Level 0, it's likely you'll directly proceed.

4.  **Enter Username and Server Details:** The command automatically specifies the username (`bandit0`) and server address (`bandit.labs.overthewire.org`) and port (`2220`).

5.  **Successful Connection Attempted:**  After executing the command, the terminal output will attempt to connect to the Bandit server.

---

## 📸 Visual Evidence: Terminal Showing SSH Command & Connection Attempt

![Terminal Showing SSH Command & Connection Attempt](images/terminal_output_level0.png)
*(Screenshot visually confirming the SSH command entered and the server prompting for a password, indicating a connection attempt.)*

-----

## 🔑 Key Learnings & Skills Demonstrated

Completing Bandit Level 0 provided valuable foundational learning and demonstrated the following skills relevant to cybersecurity and technical roles:

  * **Fundamental SSH Usage:**  Successfully utilized the `ssh` command to initiate a remote connection attempt.
  * **Understanding of Ports:**  Reinforced that SSH operates on specific ports (default 22, here 2220) and how to specify non-default ports using the `-p` flag.
  * **Command-Line Proficiency:**  Reinforced basic command-line interaction, essential for Linux environments and cybersecurity tasks.
  * **Problem-Solving in a Cybersecurity Context:** Successfully followed instructions and initiated a connection to a secure server for a cybersecurity objective.

-----

## 🚀 Next Steps: Level 1 and Beyond\!

Excited to continue progressing through the OverTheWire Bandit challenges\! Level 1 and beyond will further develop my cybersecurity skillset and command-line expertise. Stay tuned for more updates on my CTF journey\! 🔥

-----
