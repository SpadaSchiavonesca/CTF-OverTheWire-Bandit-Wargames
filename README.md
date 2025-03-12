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
    ssh bandit2@bandit.labs.overthewire.org -p 2220
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

![Terminal Showing File Listing and Reading "spaces in this filename"](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-17-14.png?raw=true)
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
# 🛡️ OverTheWire Bandit CTF - Level 3: Discovering Hidden Files 🕵️‍♂️

## Expanding File System Skills: Unveiling Hidden Directories

Building upon file system navigation and password authentication, this document details my completion of **Bandit Level 3**.  This level focuses on expanding **file system exploration skills** to discover **hidden directories and files**, a common technique in cybersecurity to conceal sensitive information and test a user's ability to thoroughly investigate a system.

-----

## Challenge Overview: Uncovering Hidden Content 🚩

**OverTheWire Bandit** continues its progressive approach to teaching Linux command-line and cybersecurity skills. Level 3 challenges participants to go beyond basic file listings and utilize specific command options to reveal hidden content within the Linux file system.

**Level 3 Objective:** Locate a hidden directory within the `bandit3` user's home directory, and within it, find and read a file to obtain the password for Bandit Level 4.

-----

## ✅ Steps to Complete Bandit Level 3

Here are the steps I took to successfully complete Bandit Level 3:

1.  **Establish SSH Connection to Bandit Level 3:** Log in to the Bandit server as user `bandit3`.  *(Password for `bandit3` is obtained from Bandit Level 2 - refer to Level 2 documentation.)*

    ```bash
    ssh bandit3@bandit.labs.overthewire.org -p 2220
    ```

2.  **List All Files and Directories, Including Hidden Ones (`ls -a` command):** Once logged in, I used the `ls -a` command. The `-a` option is crucial as it instructs `ls` to display *all* entries in the directory, including hidden files and directories (those whose names begin with a dot `.`).

    ```bash
    ls -a
    ```

3.  **Identify the Hidden Directory:** By examining the output of `ls -a`, I looked for directory names starting with a dot (`.`). I identified the hidden directory name. *(The specific name is part of the challenge.)*

4.  **Navigate to the Hidden Directory (`cd` command):** I used the `cd` command to change my current directory to the hidden directory found in the previous step.

    ```bash
    cd [hidden_directory_name]
    ```
    *(Replace `[hidden_directory_name]` with the actual name of the hidden directory.)*

5.  **List Files in the Hidden Directory (`ls` command):**  Within the hidden directory, I used `ls` to list its contents and identify the file containing the password.

    ```bash
    ls
    ```

6.  **Read the Password File (`cat` command):** Finally, I used the `cat` command to read the contents of the file found within the hidden directory. This file contained the password for Bandit Level 4.

    ```bash
    cat [password_filename]
    ```
    *(Replace `[password_filename]` with the actual filename containing the password.)*

7.  **Extract Bandit Level 4 Password:** The `cat` command displayed the Bandit Level 4 password, which I then noted for the next level.

8.  **Logout (Optional):**  Used the `exit` command to close the SSH connection.

    ```bash
    exit
    ```

-----

## 📸 Visual Guide: Terminal Showing SSH Login Attempt to Bandit Level 3

![Terminal Showing SSH Login Attempt to Bandit Level 3](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-24-33.png?raw=true)
![Terminal Showing SSH Login Attempt to Bandit Level 3](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-25-48.png?raw=true)
![Terminal Showing SSH Login Attempt to Bandit Level 3](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-31-57.png?raw=true)
![Terminal Showing SSH Login Attempt to Bandit Level 3](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-33-44.png?raw=true)
<center>*(Screenshot showing the initial SSH login attempt to Bandit Level 3.  This might show the password prompt or a "Connection closed" message if the password was incorrect, as seen in this example.)*</center>

-----

## 🔑 Key Learnings & Skills Demonstrated in Level 3

Completing Bandit Level 3 further developed my Linux command-line skills and demonstrated:

  * **Hidden File Discovery:**  Successfully utilized the `ls -a` command to reveal and identify hidden files and directories, a critical skill in Linux security and system administration.
  * **File System Navigation:**  Continued to practice and refine file system navigation using `ls` and `cd` commands.
  * **Command-Line Options:** Learned the importance and usage of command-line options like `-a` to modify command behavior and reveal more information.
  * **Problem-Solving Strategies:**  Applied a systematic approach to exploring the file system and locating the hidden password, building problem-solving skills in a CTF context.
  * **Progressive Learning:**  Demonstrated continued progression through the Bandit challenges, building upon skills from previous levels.

-----

## 🚀 Next Steps: Level 4 and Beyond\!

Equipped with the ability to uncover hidden files and directories, I am now ready to advance to Bandit Level 4 and further explore the OverTheWire Bandit challenges\!  Each level is enhancing my cybersecurity knowledge and command-line proficiency. Stay tuned for more updates on my CTF journey\! 🔥

-----
# 🛡️ OverTheWire Bandit CTF - Level 4: Finding the Right File Type 🔍

## Expanding File System Skills: Identifying Files by Type

Continuing my progression through the Bandit challenges, this document details my completion of **Bandit Level 4**. This level further develops **file system skills** by requiring the use of the `file` command to **identify files based on their type**. This is a fundamental skill in system administration and security analysis for understanding and categorizing different data formats.

-----

## Challenge Overview: File Type Identification 🚩

**OverTheWire Bandit** Level 4 builds upon previous file system navigation skills by introducing the concept of file types. The challenge requires using the `file` command to differentiate between various file types and locate a specific file type containing the password for the next level.

**Level 4 Objective:** In the `bandit4` user's home directory, there's a directory named `inhere`.  Within `inhere`, there are multiple files. Identify the one file that is of type "text" (ASCII text) and read its contents to obtain the password for Bandit Level 5.

-----

## ✅ Steps to Complete Bandit Level 4

Here are the steps I took to successfully complete Bandit Level 4:

1.  **Establish SSH Connection to Bandit Level 4:** Log in to the Bandit server as user `bandit4`.  *(Password for `bandit4` is obtained from Bandit Level 3 - refer to Level 3 documentation.)*

    ```bash
    ssh bandit4@bandit.labs.overthewire.org -p 2220
    ```

2.  **List Files and Directories in Home Directory (`ls -a` command):** Once logged in, I used `ls -a` to see all files and directories.  This revealed a directory named `inhere`.

    ```bash
    ls -a
    ```

3.  **Navigate to the `inhere` Directory (`cd inhere` command):** I used the `cd inhere` command to change my current directory to the `inhere` directory.

    ```bash
    cd inhere
    ```

4.  **List Files in `inhere` Directory (`ls -l` command):**  Inside the `inhere` directory, I used `ls -l` to get a detailed listing of all files. This showed files named `-file00`, `-file01`, ..., `-file09`.

    ```bash
    ls -l
    ```

5.  **Determine File Types (`file ./-file*` command):** To determine the type of each file, I used the `file` command with a wildcard `./-file*` to check all files starting with `-file`. The `./` is important to specify that the files are in the current directory due to the filenames starting with `-`.

    ```bash
    file ./-file*
    ```
    *(This command examines each file and outputs its file type.)*

6.  **Identify the "ASCII text" File:**  From the output of the `file` command, I scanned the results to identify the file that was reported as "ASCII text".  In this case, it was `-file07`.

7.  **Read the Password File (`cat ./-file07` command):**  Once I identified `-file07` as the ASCII text file, I used the `cat` command to read its contents.  Again, `./` is used before `-file07` because of the leading hyphen in the filename.

    ```bash
    cat ./-file07
    ```

8.  **Extract Bandit Level 5 Password:** The `cat` command displayed the password for Bandit Level 5, which I carefully noted.

9.  **Logout (Optional):** Used the `exit` command to close the SSH connection.

    ```bash
    exit
    ```

-----

## 📸 Visual Guide: Terminal Showing File Type Identification in Level 4

![Terminal Showing File Type Identification for Bandit Level 4](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-49-21.png?raw=true)
![Terminal Showing File Type Identification for Bandit Level 4](https://github.com/SpadaSchiavonesca/CTF-OverTheWire-Bandit-Wargames/blob/main/Screenshots/Screenshot_2025-03-11_19-51-58.png?raw=true)
<center>*(Screenshot demonstrating the process of listing files, navigating to the `inhere` directory, listing files within `inhere`, and crucially, using the `file` command to identify the file type of each `-fileXX` file. The output of `file ./-file*` clearly shows `-file07` as "ASCII text".)*</center>

-----

## 🔑 Key Learnings & Skills Demonstrated in Level 4

Completing Bandit Level 4 significantly expanded my Linux command-line skills and demonstrated:

  * **File Type Identification:** Successfully used the `file` command to determine the type of various files.  This is a vital skill for system analysis, security, and scripting.
  * **Advanced File System Navigation:**  Practiced navigating directories using `cd` and listing files using `ls -a` and `ls -l` in a more complex scenario with multiple files.
  * **Understanding Filenames with Special Characters:**  Learned how to handle filenames starting with hyphens (`-`) by using `./` to correctly reference them in commands.
  * **Command Combination for Problem Solving:**  Effectively combined `ls`, `cd`, `file`, and `cat` commands in a logical sequence to solve the challenge.
  * **Progressive Skill Development:**  Continued to build upon previously learned skills, adding file type identification to my growing command-line toolkit.

-----

## 🚀 Next Steps: Level 5 and Beyond\!

With the ability to identify file types and navigate more complex file structures, I am now well-prepared to advance to Bandit Level 5 and continue my learning journey through the OverTheWire Bandit challenges\! Each level further enhances my cybersecurity and Linux command-line expertise. Stay tuned for more updates on my CTF progress\! 🔥

-----
