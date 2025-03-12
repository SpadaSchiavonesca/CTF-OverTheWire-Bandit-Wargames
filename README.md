# Capture The Flag: OverTheWire Bandit Challenges 🛡️

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
![Terminal Showing SSH Command & Connection Attempt](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-07-11.png?.pngraw=true)
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

## 📸 Visual Guide: Terminal Showing Bandit Level 1 MOTD & Password Location

![Terminal Showing SSH Command & Connection Attempt](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-10-25.png?.pngraw=true)
![Terminal Showing SSH Command & Connection Attempt](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-10-54.png?.pngraw=true)
![Terminal Showing SSH Command & Connection Attempt](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-14-08.png?.pngraw=true)
![Terminal Showing SSH Command & Connection Attempt](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-14-27.png?.pngraw=true)
<center>*(Screenshot visually confirming the SSH command entered and the server prompting for a password, indicating a connection attempt.)*</center>

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
# 🛡️ OverTheWire Bandit CTF - Level 2: Accessing Files with Spaces 📂

## Mastering Basic File System Navigation and Handling Special Characters

Having successfully authenticated via SSH in Level 1, this document details my progression to **Bandit Level 2**.  This level introduces fundamental **file system navigation** within the Linux command-line environment and specifically focuses on **handling filenames that contain spaces and special characters**, a common scenario in real-world systems.

-----

## Challenge Overview: Expanding Linux Command-Line Skills 🚩

**OverTheWire Bandit** continues its progressive approach, with Level 2 challenging participants to interact with the file system and overcome obstacles like filenames with spaces.  This level is crucial for building practical command-line proficiency and understanding how to work with files in Linux environments.

**Level 2 Objective:** Locate and read the contents of a file named "spaces in this filename" within the `bandit2` user's home directory to obtain the password for Bandit Level 3.

-----

## ✅ Steps to Complete Bandit Level 2

Here are the steps I took to successfully complete Bandit Level 2:

1.  **Establish SSH Connection to Bandit Level 2:** Log in to the Bandit server as user `bandit2`.  *(Password for `bandit2` is obtained from Bandit Level 1 - refer to Level 1 documentation.)*

    ```bash
    ssh [email address removed] -p 2220
    ```

2.  **List Files in Home Directory (`ls` command):**  Once logged in, used the `ls` command to list the files and directories in the current working directory (which defaults to the `bandit2` user's home directory upon login).

    ```bash
    ls
    ```
    *(This command reveals the contents of the current directory, allowing identification of the target file.)*

3.  **Identify the File with Spaces:** From the output of the `ls` command, identified the filename "spaces in this filename".  *(Note the spaces within the filename, which require special handling in the command line.)*

4.  **Read the File Content (`cat` command with Filename Escaping):** Utilized the `cat` command to read the content of the "spaces in this filename" file.  Crucially, the spaces in the filename were escaped using backslashes (`\`) to ensure the shell correctly interpreted the filename as a single argument:

    ```bash
    cat spaces\ in\ this\ filename
    ```
    *(The backslashes escape the spaces, preventing the shell from interpreting "spaces", "in", "this", and "filename" as separate arguments.)*

5.  **Extract Bandit Level 3 Password:** The output of the `cat` command displayed the password for Bandit Level 3.  Carefully copied or noted down this password.

6.  **Logout (Optional):** Used the `exit` command to close the SSH connection to Bandit Level 2.

    ```bash
    exit
    ```

-----

## 📸 Visual Guide: Terminal Showing File Listing and Reading with `cat`

![Terminal Showing File Listing and Reading "spaces in this filename"](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_20-46-50.png?raw=true)
<center>*(Screenshot illustrating the use of the `ls` command to list files, identifying "spaces in this filename", and then using the `cat` command with backslash escaping to read the file's contents and reveal the Bandit Level 3 password.)*</center>

-----

## 🔑 Key Learnings & Skills Demonstrated in Level 2

Completing Bandit Level 2 significantly enhanced my Linux command-line skills and demonstrated the following:

  * **Basic File System Navigation:**  Utilized the `ls` command for fundamental file system exploration and listing directory contents.
  * **Handling Filenames with Spaces:** Mastered the technique of using backslashes (`\`) to escape spaces in filenames when using command-line tools like `cat`.  *(This is a common requirement when working with real-world file systems.)*
  * **`cat` Command Usage:**  Reinforced the use of the `cat` command for viewing the contents of files.
  * **Command-Line Argument Handling:**  Developed a better understanding of how the Linux shell parses commands and arguments, and the importance of escaping special characters.
  * **Progressive Skill Building:**  Successfully built upon previous SSH login skills and expanded into file system interaction, demonstrating a progressive learning approach.

-----

## 🚀 Next Steps: Level 3 and Beyond\!

Having successfully navigated filenames with spaces in Level 2, I am eager to progress to Level 3 and continue expanding my Linux command-line and cybersecurity skillset through the OverTheWire Bandit challenges\! Stay tuned for more updates on my CTF journey\! 🔥

-----
