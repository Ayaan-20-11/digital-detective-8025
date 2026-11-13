# Mission 3: Operating Systems

## 1. Task / Objective

The objective of this mission was to explore the operating system, inspect running processes, understand file paths and permissions, and learn the major responsibilities of an operating system.

I performed these activities on macOS using the Terminal.

## 2. Work Completed

### Task 3.1 — Exploring the Operating System

I used Terminal commands to inspect my operating system, account information, available storage, and running system activity.

| Information explored | What it tells me | My observation |
|---|---|---|
| Operating system | Identifies the installed operating system and its version. | macOS, version 27.2, build 26B123. |
| Current account | Identifies the account currently using the system. | The command displayed my account username. I have kept it private and redacted it. |
| Available storage | Shows total, used, and available disk space. | 926 GiB total, 174 GiB used, 715 GiB available, with 20% capacity used. |
| System activity | Shows running and sleeping processes, CPU usage, and memory usage. | The snapshot showed 792 processes: 2 running and 790 sleeping. CPU usage was 11.8% user, 12.23% system, and 76.67% idle. |

### Task 3.2 — Understanding Processes

A process is an instance of a program that is currently running on a computer. Each process is assigned a unique Process ID (PID), which helps the operating system identify and manage it.

I used the `ps aux | head -10` command to view a snapshot of running processes.

**What does the PID column represent?**

PID stands for Process ID. It is a unique numerical identifier assigned to each running process by the operating system.

**Two examples of processes I observed:**

1. Brave Browser Helper (Renderer) — a process responsible for rendering browser content.
2. Code Helper (Renderer) — a process associated with the Visual Studio Code interface.

I also observed that a single application can use multiple processes for different tasks.

### Task 3.3 — Understanding Paths and Permissions

I used `pwd` to identify my current working directory and `cd` to navigate into the Mission 3 folder.

**Absolute path:**

An absolute path specifies the complete location of a file or folder, starting from the root directory.

Example:

`/Users/[redacted]/Desktop/digital-detective-8025/mission-03-operating-system`

**Relative path:**

A relative path specifies a location in relation to the current working directory.

Example:

`mission-03-operating-system`

This path can be used from the repository root to access the Mission 3 folder.

I also used the following command to inspect a file created during Mission 2:

`ls -l ../terminal-practice/notes.txt`

The output showed the permission string:

`-rw-r--r--`

**Understanding the permissions:**

- `-` indicates that it is a regular file.
- `rw-` means the owner can read and write the file but cannot execute it.
- `r--` means the group can only read the file.
- `r--` means other users can only read the file.

I understood that file permissions help the operating system control who can access or modify files.

### Task 3.4 — Responsibilities of an Operating System

| Responsibility | Explanation | Example |
|---|---|---|
| Process management | Manages running programs and allocates CPU time to them. | Managing Brave Browser and VS Code processes. |
| Memory management | Allocates and manages RAM used by different applications. | Providing memory to Brave Browser and VS Code while they run. |
| Device management | Controls and coordinates hardware devices using drivers and system services. | Managing audio input and output through macOS audio services. |
| File management | Organises files and folders and manages how they are stored and accessed. | Saving and opening `notes.txt` inside the assignment folder. |
| User interface / shell | Allows users to interact with the computer through a graphical interface or command line. | Using the macOS desktop and Terminal. |
| Security and permissions | Controls access to files and system resources. | Using file permissions to determine who can read or modify a file. |

## 3. Commands / Tools Used

The following commands were used during this mission:

| Command | Purpose |
|---|---|
| `sw_vers` | Displays macOS version information. |
| `whoami` | Displays the current account username. |
| `df -h .` | Displays disk storage information in a readable format. |
| `top -l 1 -n 5` | Displays a snapshot of system activity and processes. |
| `ps aux \| head -10` | Displays the first ten lines of the running process list. |
| `pwd` | Displays the current working directory. |
| `cd mission-03-operating-system` | Navigates into the Mission 3 directory. |
| `ls -l ../terminal-practice/notes.txt` | Displays detailed file information, including permissions. |

**Tools used:** macOS, Terminal, and Visual Studio Code.

## 4. My Understanding

Through this mission, I understood that an operating system acts as an interface between the user, applications, and computer hardware.

I learned how to inspect system information, observe running processes, understand process IDs, navigate using absolute and relative paths, and interpret file permissions.

I also understood that an operating system manages important resources such as CPU time, memory, storage, and connected devices while providing security and a user interface.

## 5. Difficulties Faced

Initially, I found it slightly confusing to distinguish between absolute and relative paths. Understanding the different groups of file permissions was also new to me.

## 6. How I Resolved Them

I practised navigating between the repository root and the Mission 3 directory using `pwd` and `cd`. I also inspected an existing practice file using `ls -l` and studied the permission string character by character.

These practical exercises helped me understand the concepts more clearly.

## 7. Evidence / Files

- Mission 3 README documenting the tasks and observations.
- Terminal commands and their outputs were used to verify system information, process activity, paths, and file permissions.
- The practice file `terminal-practice/notes.txt` from Mission 2 was used to inspect file permissions.

Personal account details and identifying information have been redacted from the documentation.

## 8. Commit Details

- Commit message: `Document operating system and file management`
- Changes pushed to the GitHub repository after completing Mission 3.
