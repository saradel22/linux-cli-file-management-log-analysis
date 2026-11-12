# Command examples used in the project

Run from `~/linux-cli-project` unless otherwise noted. These are reference examples from the practical exercises, not a complete exported Bash history.

## System information

```bash
whoami
pwd
cat /etc/os-release
hostname
ls -al
```

## Navigation and files

```bash
mkdir -p ~/linux-cli-project/{documents,logs,reports,backups}
cd ~/linux-cli-project
ls -al
# From inside documents/:
touch notes.txt tasks.txt draft.txt
cp notes.txt ../backups/
mv draft.txt final.txt
mv tasks.txt ../reports/
touch test.txt
rm test.txt
```

## Links

```bash
ln -s documents/notes.txt notes-shortcut.txt
ln documents/notes.txt notes-hardlink.txt
ls -li documents/notes.txt notes-shortcut.txt notes-hardlink.txt
```

## Reading and searching sample logs

```bash
cat logs/application.log
head -n3 logs/application.log
tail -n2 logs/application.log
wc -l logs/application.log
grep -i error logs/application.log
grep -i warning logs/application.log
grep -in error logs/application.log
find . -name '*.log'
```

## Output redirection

```bash
uname -a > reports/system.txt
date >> reports/system.txt
ls missingfolder 2> reports/errors.txt
ls documents missingfolder > reports/combined.txt 2>&1
```

## Text processing

```bash
grep -ic error logs/application.log
sort logs/application.log
cut -d ' ' -f2 logs/application.log | sort | uniq
cut -d ' ' -f2 logs/application.log | sort | uniq -c
cut -d ' ' -f2 logs/application.log
tr 'a-z' 'A-Z' < logs/application.log
cat logs/application.log | tee reports/log-copy.txt
cat logs/application.log | tee -a reports/log-copy.txt
paste documents/notes.txt logs/application.log
```
