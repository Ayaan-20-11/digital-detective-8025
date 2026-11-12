# Mission 2: Terminal and File Management

## 1. Task / Objective

The objective of this mission was to understand and practise basic Command Line Interface (CLI) operations using macOS Terminal. I explored directory navigation, file creation, copying, renaming, modifying files, command-line flags, pipes and package managers.

## 2. Work Completed

### Task 2.1: Basic Terminal Operations

I performed the following operations inside my assignment repository:

| Operation | Command Used | What I Observed |
|---|---|---|
| Display current directory | `pwd` | Displayed the full path of my current working directory. |
| List files and folders | `ls` | Displayed the visible files and directories in the repository. |
| Detailed listing | `ls -l` | Displayed permissions, ownership, file sizes and modification dates. |
| Move to parent directory | `cd ..` | Moved from the repository directory to its parent directory, Desktop. |
| Create a practice folder | `mkdir terminal-practice` | Created a new directory inside the repository. |
| Create an empty text file | `touch terminal-practice/notes.txt` | Created an empty file named notes.txt. |
| Copy a file | `cp terminal-practice/notes.txt terminal-practice/notes-copy.txt` | Created a separate copy while keeping the original file. |
| Rename a file | `mv terminal-practice/notes-copy.txt terminal-practice/renamed-notes.txt` | Renamed the copied file. |
| Display file contents | `cat terminal-practice/notes.txt` | Displayed the text stored inside the original file. |

### Task 2.2: Safe File Management

I created and modified files inside the `terminal-practice` directory.

Commands used:

```bash
echo "This is my original practice file." > terminal-practice/notes.txt

echo "This is the second line added using append." >> terminal-practice/notes.txt

cat terminal-practice/notes.txt

cp terminal-practice/notes.txt terminal-practice/notes-backup.txt

mv terminal-practice/notes-backup.txt terminal-practice/notes-backup-final.txt

ls terminal-practice
```

The final directory contained:

- `notes.txt`
- `renamed-notes.txt`
- `notes-backup-final.txt`

**Understanding the operations:**

- **Replacing contents (`>`):** Writes new content to a file and replaces its existing contents.
- **Appending (`>>`):** Adds new content at the end of a file without removing previous content.
- **Copying (`cp`):** Creates a duplicate while preserving the original file.
- **Moving (`mv`):** Changes the location or name of a file.
- **Current directory (`pwd`):** Helps identify where commands are being executed.
- **Directory listing (`ls`):** Helps inspect available files and folders before performing operations.

I verified that both lines were preserved after appending by displaying the file with `cat`.

### Task 2.3: Command Flags and Pipes

I experimented with different flags using the `ls` command.

| Command | Purpose | Observation |
|---|---|---|
| `ls` | Normal listing | Displayed visible files and directories. |
| `ls -l` | Detailed listing | Displayed permissions, ownership, sizes and dates. |
| `ls -a` | Include hidden files | Revealed hidden entries such as `.git`, `.` and `..`. |
| `ls -lh` | Human-readable sizes | Displayed file sizes using units such as B and K. |
| `ls -lah` | Combine flags | Displayed hidden files, detailed information and human-readable sizes. |

**Understanding pipes:**

I executed:

```bash
ls -l | head -5
```

The pipe symbol (`|`) passes the output of the first command as input to the next command.

- `ls -l` generates a detailed directory listing.
- `head -5` displays the first five lines of that output.

This demonstrated how multiple commands can be connected to process output efficiently.

### Task 2.4: Package Managers

I checked whether Homebrew was installed on my Mac.

Command:

```bash
brew --version
```

Observed output:

```text
Homebrew 7.0.8
```

I then listed the packages managed by Homebrew using:

```bash
brew list
```

The output displayed installed formulae, including packages such as Node, Python, OpenJDK, Git LFS, Ripgrep and SQLite.

**Why package managers are useful:**

A package manager helps users install, update and manage software packages from a central system. Homebrew simplifies software management on macOS by allowing users to perform these operations through Terminal commands.

No packages were installed, upgraded or uninstalled during this task.

## 3. Commands / Tools Used

- `pwd` — Display current working directory.
- `ls` — List directory contents.
- `ls -l` — Display detailed listing.
- `ls -a` — Include hidden files.
- `ls -lh` — Display human-readable sizes.
- `ls -lah` — Combine listing options.
- `cd ..` — Move to parent directory.
- `mkdir` — Create a directory.
- `touch` — Create an empty file.
- `cp` — Copy a file.
- `mv` — Move or rename a file.
- `echo` — Print text.
- `>` — Redirect output and replace file contents.
- `>>` — Append output to a file.
- `cat` — Display file contents.
- `head -5` — Display the first five lines.
- `|` — Connect commands using a pipe.
- `brew --version` — Check Homebrew version.
- `brew list` — List Homebrew-managed formulae.

## 4. My Understanding

This mission helped me understand how to interact with the operating system through Terminal instead of relying entirely on a graphical interface.

I learned how directory navigation works, how files can be created and modified, and how commands such as `cp` and `mv` perform different operations.

I also understood that command-line flags modify the behaviour of commands, while pipes allow the output of one command to be processed by another.

Finally, I explored Homebrew and understood how package managers simplify software management.

## 5. Difficulties Faced

Initially, I needed to understand how to navigate between the repository directory and its parent directory. I also needed to distinguish between copying a file and renaming it.

Another important concept was understanding the difference between overwriting file contents and appending new content.

## 6. How I Resolved Them

I practised each command individually and verified the results using commands such as `pwd`, `ls` and `cat`.

I compared the behaviour of `>` and `>>` by writing two lines into the same file. I also used `ls` after copying and renaming files to confirm the results.

For flags and pipes, I compared the outputs of different `ls` commands and observed how `head -5` filtered the listing.

## 7. Evidence / Files

The practical work was performed inside the `terminal-practice` directory.

Files created:

- `terminal-practice/notes.txt`
- `terminal-practice/renamed-notes.txt`
- `terminal-practice/notes-backup-final.txt`

The terminal commands and their outputs served as evidence of the completed operations.

## 8. Commit Details

- Commit message: `Complete Terminal and file management mission`
- Repository: [digital-detective-8025](https://github.com/Ayaan-20-11/digital-detective-8025)
- Commit hash: To be updated after committing and pushing this mission.