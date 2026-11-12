# Project Report: Linux CLI-Based File Management and Log Analysis

## 1. Objective

Demonstrate essential Linux administration tasks through a command-line file management and sample log-analysis workflow.

## 2. Environment

- Ubuntu 26.04 LTS under WSL2
- Bash shell and standard Linux command-line tools
- Local workspace: `~/linux-cli-project`

## 3. Work performed

**Environment and navigation:** Verified the Linux username, working directory, distribution, and hostname. Explored `/usr`, `/tmp`, and project directories; practiced absolute and relative paths and directory listing options.

**File management:** Created `documents`, `logs`, `reports`, and `backups`. Created example text files; copied a backup; renamed, moved, and removed practice files. Created and inspected a symbolic link and a hard link.

**Log inspection:** Created a five-line sample application log containing INFO, ERROR, and WARNING events. Used command-line tools to view full content, view selected lines, count lines, locate keywords, and discover `.log` files.

**Redirection:** Practiced `>`, `>>`, `2>`, and `2>&1` for saving outputs and errors to files. A report-file correction was identified during review; verify `reports/system.txt` and `reports/errors.txt` after applying the fix.

**Pipelines and processing:** Extracted the log-level field, sorted and deduplicated entries, counted occurrences, converted text to uppercase, and saved/appended output using `tee`. Tested column-wise merging with `paste` (the comparison input was empty).

## 4. Sample results

The five sample log records contain **2 ERROR**, **2 INFO**, and **1 WARNING** entries. The sample issues were a database connection failure, high memory usage, and a permission-denied event. These observations come from the terminal screenshots and are not production incidents.

## 5. Challenges and fixes

- Corrected file paths by distinguishing the filesystem root `/` from paths relative to the project folder.
- Corrected the order of standard-output and standard-error redirections.
- Distinguished case-sensitive from case-insensitive `grep` searches.
- Verified that the symbolic link points to the expected relative file path and the hard link shares the original file's inode.

## 6. Conclusion

The project provided hands-on practice with Linux file organization, terminal navigation, output redirection, log filtering, and command pipelines, which are useful foundations for Linux server operations and cloud support troubleshooting.

## 7. Evidence

Screenshots `01`–`07` in the `screenshots/` folder show the executed terminal workflow. Original workspace files should be added separately from WSL2 before the repository is published.
