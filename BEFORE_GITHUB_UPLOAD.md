# Before you upload to GitHub

This starter bundle has your seven screenshots and the documentation. **It does not contain a verified copy of your actual WSL2 project files.**

1. In Ubuntu, from `~/linux-cli-project`, verify the Stage 4 reports:
   ```bash
   uname -a > reports/system.txt
   date >> reports/system.txt
   ls missingfolder 2> reports/errors.txt
   ```
2. Open the Linux project folder in Windows Explorer:
   ```bash
   cd ~/linux-cli-project
   explorer.exe .
   ```
3. Extract this ZIP on Windows. Copy the **actual** `documents/`, `logs/`, `reports/`, `backups/`, and link files from the Explorer window into the extracted folder. Windows may not preserve Linux symbolic and hard links correctly when copied; if that happens, omit those two link entries and rely on the screenshot + command documentation instead.
4. Review the screenshots for any identifying information you do not want public. Do not publish passwords, tokens, or secrets.
5. Upload the finished folder to a new GitHub repository named `linux-cli-file-management-log-analysis` using **Add file → Upload files**. Commit the files.

A guided project should be identified as guided; the README already does this.
