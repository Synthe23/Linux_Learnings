🐧 Mini Linux DevOps Project: Server Setup & Log Management

Level: Beginner
•⁠  ⁠Estimated Time: 2 Hours
•⁠  ⁠Domain: Linux System Administration / DevOps
•⁠  ⁠Environment: Ubuntu Linux
•⁠  ⁠Approach: Hands-on, command-line practice
•⁠  ⁠Objective: Learn how Linux commands are used in real-world DevOps tasks.


📌 1. Project Overview

Your company has a small Node.js application called "myapp". Your senior DevOps engineer has asked you to prepare a Linux environment for this application.

Your responsibilities include:

•⁠  ⁠Creating a proper directory structure.
•⁠  ⁠Managing users and groups.
•⁠  ⁠Creating and organizing application files.
•⁠  ⁠Configuring file permissions and ownership.
•⁠  ⁠Searching and filtering application logs.
•⁠  ⁠Monitoring disk usage and running processes.
•⁠  ⁠Generating a basic server report.

🎯 Project Objective

Complete all the tasks using Linux commands through the terminal.

---

⏱️ 2. Project Time Allocation

Part| Task| Estimated Time
1| Server Initialization| 15 min
2| User and Group Management| 20 min
3| File and Directory Management| 20 min
4| File Permissions and Ownership| 20 min
5| Application Log Management| 25 min
6| Process and Disk Monitoring| 15 min
7| Final Server Report| 5 min
| Total| 120 min

---

🛠️ 3. Project Tasks

Part 1 – Server Initialization (15 Minutes)

Situation: You've just logged into a new Linux server. Before doing anything, you need to understand the environment.

Questions

1.1. Display the current logged-in username.
1.2. Display the current working directory.
1.3. Display the Linux system information, including the kernel version.
1.4. Display the current date and time.
1.5. List all files and directories, including hidden files, in the current directory.
1.6. Create a directory called "devops-project" inside your home directory.
1.7. Navigate into the newly created directory.
1.8. Display the absolute path of your current directory.

Expected Outcome

You understand your Linux environment and have created your project workspace.

---

Part 2 – User and Group Management (20 Minutes)

Situation: Your application team has two members:

•⁠  ⁠"developer1" – Responsible for application development.
•⁠  ⁠"tester1" – Responsible for application testing.

You need to create their accounts and organize their access.

Questions

2.1. Create a group named "devteam".
2.2. Create a user named "developer1".
2.3. Create another user named "tester1".
2.4. Add both users to the "devteam" group.
2.5. Display all groups associated with "developer1".
2.6. Display information about both users.
2.7. Check the current logged-in user's groups.
2.8. Find the group ID (GID) of "devteam".

Expected Outcome

Both team members exist and belong to the correct group.

---

Part 3 – File and Directory Management (20 Minutes)

Situation: The development team wants a structured directory for the application.

Required Directory Structure

Create the following directory structure:

devops-project/
│
├── myapp/
│   ├── src/
│   ├── logs/
│   ├── config/
│   └── backup/
│
├── scripts/
│
└── reports/

Questions

3.1. Create the complete directory structure.
3.2. Navigate into the "myapp" directory.

3.3. Create three files:
•⁠  ⁠"app.js" inside "src".
•⁠  ⁠"server.log" inside "logs".
•⁠  ⁠"app.conf" inside "config".

3.4. Add the following content to "app.js":
console.log("Application started");
console.log("Server running on port 3000");

3.5. Add the following configuration details to "app.conf":
APP_NAME=myapp
PORT=3000
ENVIRONMENT=development

3.6. Display the contents of "app.js".
3.7. Display the contents of "app.conf".
3.8. Copy "app.conf" into the "backup" directory.
3.9. Rename the backup copy to "app-backup.conf".
3.10. Display the complete directory structure.

Expected Outcome

Your application directory is ready with the required files.

---

Part 4 – File Permissions and Ownership (20 Minutes)

Situation: Your senior engineer has informed you that not every team member should have access to every application file.

You need to configure permissions properly.

Questions

4.1. Display the permissions of all files inside "myapp".
4.2. Give the owner read, write and execute permissions on "app.js".
4.3. Give the group read and write permissions on "app.js".
4.4. Remove all permissions from other users on "app.js".
4.5. Change the ownership of the "myapp" directory to "developer1".
4.6. Change the group ownership of the application directory to "devteam".
4.7. Give the "logs" directory appropriate permissions so that the owner and group can access it.
4.8. Verify the permissions and ownership changes.

Expected Outcome

Application files are accessible to the correct users.

DevOps Learning Point: Understand the difference between "chmod", "chown", and "chgrp".

---

Part 5 – Application Log Management (25 Minutes)

Situation: Your application has started running, but the development team reports some errors.

Your job is to inspect the logs and identify the issues.

Step 1: Populate the Log File

Add the following sample data to "server.log":

[INFO] Server started successfully
[INFO] Application running on port 3000
[WARNING] High memory usage detected
[ERROR] Database connection failed
[INFO] Retrying database connection
[ERROR] Authentication service unavailable
[INFO] Database connected successfully
[WARNING] Disk usage above 80%
[ERROR] Request timeout occurred
[INFO] Server running normally

Step 2: Log Analysis Questions

5.1. Display the complete log file.
5.2. Display only the first five lines.
5.3. Display only the last five lines.
5.4. Search for all occurrences of "ERROR" in the log file.
5.5. Search for all occurrences of "WARNING".
5.6. Count the total number of lines in the log file.
5.7. Count how many errors occurred.
5.8. Display the log file with line numbers.
5.9. Search for the word "Database" without worrying about uppercase or lowercase letters.
5.10. Continuously monitor the log file as new entries are added.
5.11. Add a new entry to the log file:

[ERROR] Payment service failed

5.12. Verify that the new error appears in your log file.

Expected Outcome
You can inspect, filter, count and monitor application logs.
DevOps Learning Point: Log analysis is one of the most frequently used Linux skills in production environments.

---

Part 6 – Process and Disk Monitoring (15 Minutes)

Situation: The application is running, but your senior engineer wants you to check the server's resource usage.

Questions

6.1. Display all currently running processes.
6.2. Find processes associated with your terminal session.
6.3. Display real-time CPU and memory usage.
6.4. Check available disk space on the server.
6.5. Check the size of the "devops-project" directory.
6.6. Display memory usage in a human-readable format.
6.7. Display the last few commands executed in your terminal.

Expected Outcome

You can perform basic Linux server monitoring.

---

Part 7 – Final Server Report (5 Minutes)

Situation: Your senior engineer wants a quick report of your server setup.

Create a file named "server-report.txt" inside the "reports" directory.

Questions

7.1. Write the current date and time into the report.
7.2. Add the current username.
7.3. Add the total number of files inside your project.
7.4. Add the disk usage information.
7.5. Add the memory usage information.
7.6. Display the completed report.

Final Expected Directory Structure

devops-project/
│
├── myapp/
│   ├── src/
│   │   └── app.js
│   │
│   ├── logs/
│   │   └── server.log
│   │
│   ├── config/
│   │   └── app.conf
│   │
│   └── backup/
│       └── app-backup.conf
│
├── scripts/
│
└── reports/
    └── server-report.txt

---

📚 4. Linux Command Checklist

As you complete the project, try to use these commands without looking up their syntax.

System Information

•⁠  ⁠[ ] "whoami"
•⁠  ⁠[ ] "pwd"
•⁠  ⁠[ ] "uname"
•⁠  ⁠[ ] "date"
•⁠  ⁠[ ] "ls"

Users and Groups

•⁠  ⁠[ ] "groupadd"
•⁠  ⁠[ ] "useradd"
•⁠  ⁠[ ] "usermod"
•⁠  ⁠[ ] "id"
•⁠  ⁠[ ] "groups"
•⁠  ⁠[ ] "getent"

Files and Directories

•⁠  ⁠[ ] "mkdir"
•⁠  ⁠[ ] "cd"
•⁠  ⁠[ ] "touch"
•⁠  ⁠[ ] "cat"
•⁠  ⁠[ ] "echo"
•⁠  ⁠[ ] "cp"
•⁠  ⁠[ ] "mv"
•⁠  ⁠[ ] "find"
•⁠  ⁠[ ] "tree"

Permissions and Ownership

•⁠  ⁠[ ] "chmod"
•⁠  ⁠[ ] "chown"
•⁠  ⁠[ ] "chgrp"
•⁠  ⁠[ ] "ls -l"

Log Management

•⁠  ⁠[ ] "head"
•⁠  ⁠[ ] "tail"
•⁠  ⁠[ ] "grep"
•⁠  ⁠[ ] "wc"
•⁠  ⁠[ ] "less"
•⁠  ⁠[ ] "tee"

Process and Resource Monitoring

•⁠  ⁠[ ] "ps"
•⁠  ⁠[ ] "top"
•⁠  ⁠[ ] "df"
•⁠  ⁠[ ] "du"
•⁠  ⁠[ ] "free"
•⁠  ⁠[ ] "history"

---

📋 5. Project Completion Checklist

Before marking the project complete, verify the following:

•⁠  ⁠[ ] Linux environment information checked.
•⁠  ⁠[ ] Project workspace created.
•⁠  ⁠[ ] Two users created successfully.
•⁠  ⁠[ ] "devteam" group created.
•⁠  ⁠[ ] Both users added to the group.
•⁠  ⁠[ ] Application directory structure created.
•⁠  ⁠[ ] Application files created successfully.
•⁠  ⁠[ ] File permissions configured.
•⁠  ⁠[ ] Ownership and group ownership configured.
•⁠  ⁠[ ] Sample application logs added.
•⁠  ⁠[ ] Log analysis completed.
•⁠  ⁠[ ] Process monitoring performed.
•⁠  ⁠[ ] Disk and memory usage checked.
•⁠  ⁠[ ] Final server report generated.

---

🎯 6. Expected Learning Outcomes

After completing this project, you should understand how to:

1.⁠ ⁠Perform basic Linux system administration.
2.⁠ ⁠Create and manage Linux users and groups.
3.⁠ ⁠Organize application directories and files.
4.⁠ ⁠Configure file permissions and ownership.
5.⁠ ⁠Search and analyze application logs.
6.⁠ ⁠Monitor processes and system resources.
7.⁠ ⁠Generate basic server reports using Linux commands.

---

⚠️ 7. Important Rules

1.⁠ ⁠Don't copy commands directly from Google or ChatGPT. Try solving each question yourself first.
2.⁠ ⁠Use "man command" whenever you don't remember the syntax.
3.⁠ ⁠Don't skip questions, even if they seem easy.
4.⁠ ⁠Verify the output after every major operation.
5.⁠ ⁠Avoid running destructive commands such as "rm -rf" unnecessarily.
6.⁠ ⁠Use Ubuntu in a Linux VM, WSL, or another Linux environment.

Mac users: If you're practising on macOS, remember that some commands and user-management utilities differ from Ubuntu. An Ubuntu VM is recommended for this project.

---

🚀 8. What's Next?

Once you complete this project, move to the next hands-on challenge:

Project 2 – Automating Linux Server Maintenance Using Bash Scripting

You will learn to:

•⁠  ⁠Write Bash scripts.
•⁠  ⁠Automate repetitive Linux commands.
•⁠  ⁠Monitor disk and memory usage.
•⁠  ⁠Create automated backup scripts.
•⁠  ⁠Schedule tasks using Cron.
•⁠  ⁠Generate automated server health reports.

Final Advice: Don't aim for perfection. Aim to understand why and where each Linux command is used in real-world DevOps engineering.

Happy Learning! 🐧