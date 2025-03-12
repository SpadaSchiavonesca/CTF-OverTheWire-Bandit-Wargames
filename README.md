# OverTheWire Bandit Challenges 🛡️

# 🛡️ OverTheWire Bandit CTF - Level 0: SSH Connection Success 🚀

## Demonstrating Foundational Cybersecurity Skills

This document outlines my successful completion of **Bandit Level 0** from the OverTheWire Capture The Flag (CTF) challenges. OverTheWire Bandit is a fantastic resource for learning essential cybersecurity and Linux command-line skills in a gamified environment.  This level focused on establishing a fundamental skill for any cybersecurity professional: **connecting to remote servers securely via SSH.**

-----

## Challenge Overview: OverTheWire Bandit 🚩

**OverTheWire Bandit** provides a series of progressively challenging levels that teach Linux command-line expertise and core cybersecurity concepts. Starting from Level 0, the challenges are designed to be beginner-friendly and gradually introduce more complex topics.

**Level 0 Objective:** Establish a secure SSH connection to the Bandit game server.

-----

## ✅ Steps to Successful SSH Connection

Here are the steps I took to successfully complete Bandit Level 0:

1.  **Open a Terminal:** Accessed the command-line interface on my local machine (essential for interacting with remote servers).

2.  **Execute the SSH Command:** Utilized the `ssh` command, the standard tool for secure remote connections, with the specific parameters provided by OverTheWire:

    ```bash
    ssh bandit0@bandit.labs.overthewire.org -p 2220
    ```

    *(This command instructs SSH to connect to the username `bandit0` at the server address `bandit.labs.overthewire.org` using port `2220`.)*

3.  **Acknowledge Host Key (First Connection - if prompted):** Upon the initial connection, you might be prompted to acknowledge and add the server's host key. In this case, for Bandit Level 0, it's likely you'll directly proceed.

4.  **Enter Username and Server Details:** The command automatically specifies the username (`bandit0`) and server address (`bandit.labs.overthewire.org`) and port (`2220`).

5.  **Successful Connection Attempted:** After executing the command, the terminal output will attempt to connect to the Bandit server.

-----

## 📸 Visual Guide: Terminal Showing SSH Command & Connection Attempt

![Terminal Showing SSH Command & Connection Attempt](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-02-39.png?.pngraw=true)
![Terminal Showing SSH Command & Connection Attempt](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-04-01.png?.pngraw=true)
<center>*(Screenshot visually confirming the SSH command entered and the server prompting for a password, indicating a connection attempt.)*</center>

-----

## 🔑 Key Learnings & Skills Demonstrated

Completing Bandit Level 0 provided valuable foundational learning and demonstrated the following skills relevant to cybersecurity and technical roles:

  * **Fundamental SSH Usage:** Successfully utilized the `ssh` command to initiate a remote connection attempt.
  * **Understanding of Ports:** Reinforced that SSH operates on specific ports (default 22, here 2220) and how to specify non-default ports using the `-p` flag.
  * **Command-Line Proficiency:** Reinforced basic command-line interaction, essential for Linux environments and cybersecurity tasks.
  * **Problem-Solving in a Cybersecurity Context:** Successfully followed instructions and initiated a connection to a secure server for a cybersecurity objective.

-----

## 🚀 Next Steps: Level 1 and Beyond\!

Excited to continue progressing through the OverTheWire Bandit challenges\! Level 1 and beyond will further develop my cybersecurity skillset and command-line expertise. Stay tuned for more updates on my CTF journey\! 🔥

-----
# 🛡️ OverTheWire Bandit CTF - Level 1: Logging into Bandit1 🔑

## Building on Foundational SSH Skills & Introducing Password Authentication

Having successfully established an SSH connection in Level 0, this document details my progression to **Bandit Level 1**.  This level builds upon the previous challenge by introducing the crucial concept of **password-based authentication in SSH**.  It requires utilizing the SSH skills learned in Level 0 and **extracting the password for Bandit Level 1 from the Level 0 server's "message of the day" (motd).**

-----

## Challenge Overview: Progressing Through OverTheWire Bandit 🚩

**OverTheWire Bandit** continues to provide progressively challenging levels that reinforce Linux command-line expertise and core cybersecurity concepts. Level 1 specifically tests the ability to use password authentication via SSH and emphasizes the importance of information gathering within a CTF environment.

**Level 1 Objective:** Log in to the Bandit server as user `bandit1` using the password provided within the Bandit Level 0 server's message of the day (motd).

-----

## ✅ Steps to Log into Bandit Level 1 via SSH

Here are the steps I took to successfully complete Bandit Level 1:

1.  **Connect to Bandit Level 0 (if not already connected):** Establish an SSH connection to Bandit Level 0 using the command from the previous level.

    ```bash
    ssh bandit0@bandit.labs.overthewire.org -p 2220
    ```

2.  **Examine the "Message of the Day" (motd):** Carefully read the output displayed in the terminal after connecting to Bandit Level 0.  *(The motd is the server's welcome message and often contains important information in CTFs.)*

3.  **Locate the Bandit1 Password:** Within the Bandit Level 0 motd, identify the line that explicitly states the password for the *next* level (Bandit Level 1).  *(Look for text similar to: "Password for the next level bandit1 is: [your_password]")*

4.  **Open a New Terminal or SSH Session (Recommended):** Open a new terminal window or start a fresh SSH session to avoid confusion and clearly separate the Level 1 login attempt.

5.  **Execute SSH Command for Bandit Level 1:**  In the *new* terminal, utilize the `ssh` command, now targeting the `bandit1` user:

    ```bash
    ssh bandit1@bandit.labs.overthewire.org -p 2220
    ```

6.  **Enter Password When Prompted:** When prompted with `bandit1@bandit.labs.overthewire.org's password:`,  carefully type or paste the password you extracted from the Level 0 motd.

7.  **Successful Login to Bandit Level 1:** Confirm successful login when the terminal prompt changes to `bandit1@bandit:~$`, indicating you are now logged in as the `bandit1` user and ready to proceed to Level 2.

-----

## 📸 Visual Guide: Terminal Showing Bandit Level 0 MOTD & Password Location

![Terminal Showing Bandit Level 0 MOTD with Password Highlighted](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-04-01.png)
<center>*(This screenshot visually highlights the "message of the day" (motd) displayed upon successful login to Bandit Level 0. **The password for Bandit Level 1 is embedded within this motd.** Look for the line indicating the password for "the next level bandit1".)*</center>

-----

## 🔑 Key Learnings & Skills Demonstrated in Level 1

Completing Bandit Level 1 expanded my foundational cybersecurity knowledge and demonstrated the following skills:

  * **Password-Based SSH Authentication:** Successfully logged into a remote server using SSH *with* password authentication, building upon the password-less connection of Level 0.
  * **Information Gathering & Extraction:**  Developed the crucial CTF skill of carefully examining output from previous steps (Level 0 motd) to find necessary information (Level 1 password).
  * **Sequential Challenge Progression:**  Understood the sequential nature of CTF challenges and how information from one level is often required for the next.
  * **Practical SSH Command Reinforcement:**  Repeated and reinforced the use of the `ssh` command, solidifying understanding of its parameters (username, server, port).
  * **Secure Access Fundamentals:** Gained a more concrete understanding of how passwords are used to control access to remote systems via SSH.

-----

## 🚀 Next Steps: Level 2 and Beyond\!

With successful login to Bandit Level 1, I am now prepared to advance to Level 2 and continue my learning journey through the OverTheWire Bandit challenges\!  Each level is progressively building my cybersecurity skills and Linux command-line expertise. Stay tuned for more updates on my CTF progress\! 🔥

-----
