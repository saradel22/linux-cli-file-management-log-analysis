# Linux CLI-Based File Management and Log Analysis

**Guided practice project | Edureka Introduction to Linux (Coursera)**  
**Environment:** Ubuntu 26.04 LTS on Windows Subsystem for Linux (WSL2)  
**Focus:** Linux command-line administration, file operations, troubleshooting, and sample log analysis.

## Project overview

This project demonstrates practical Linux terminal workflows for organizing files, viewing and searching application logs, redirecting command output, and processing text. A small **synthetic** application log is used for demonstration; these are not logs from a production server.

## Skills demonstrated

- Navigated Linux directories and inspected system information.
- Created a structured project workspace and practiced copying, moving, renaming, and removing files.
- Created and examined symbolic and hard links.
- Inspected log files using `cat`, `head`, `tail`, and `wc`.
- Searched log entries with `grep` and found `.log` files with `find`.
- Redirected standard output and errors into report files.
- Processed text with pipelines using `cut`, `sort`, `uniq`, `tr`, `tee`, and `paste`.

## Project directory structure

```text
linux-cli-project/
├── documents/
│   ├── notes.txt
│   └── final.txt
├── logs/
│   └── application.log
├── reports/
│   ├── system.txt
│   ├── errors.txt
│   ├── combined.txt
│   └── log-copy.txt
├── backups/
│   └── notes.txt
├── notes-shortcut.txt       # symbolic link
└── notes-hardlink.txt       # hard link
```

The project files were created and tested in Ubuntu using WSL2, then copied into this GitHub repository. Some empty files are included for file-management practice.

## Example log analysis

The five-entry sample log contains:

| Level | Count |
| --- | ---: |
| ERROR | 2 |
| INFO | 2 |
| WARNING | 1 |

The example events include a failed database connection, high memory usage, and a permission-denied error. These are **simulated** events for learning.

## Commands and evidence

See [COMMANDS.md](COMMANDS.md) for commands practiced and [PROJECT_REPORT.md](PROJECT_REPORT.md) for the short project report. Terminal screenshots are in [`screenshots/`](screenshots/).

## What I learned

I practiced troubleshooting from the Linux terminal by locating files, identifying error entries, counting log events, redirecting command output, and building command pipelines to summarize text data.

## Scope

This is a **guided learning project**, not a deployed application or production monitoring system. No cloud services or paid infrastructure were required.
