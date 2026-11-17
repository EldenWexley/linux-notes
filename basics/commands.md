# Basic commands

Some commands I use regularly.

## Navigation

```bash
pwd
```
Prints the current working directory.

```bash
ls
```
Lists files and directories.

```bash
ls -la
```
Lists everything, including hidden files, with detailed information.

```bash
cd /path/to/directory
```
Changes the current directory.

```bash
cd ..
```
Moves up one directory.

```bash
cd ~
```
Returns to the home directory.

## Files and directories

```bash
mkdir test
```
Creates a directory.

```bash
touch file.txt
```
Creates an empty file if it doesn't exist.

```bash
cp file.txt backup.txt
```
Copies a file.

```bash
mv file.txt ~/Documents/
```
Moves a file.

```bash
rm file.txt
```
Deletes a file.

```bash
rmdir test
```
Removes an empty directory.

## Reading files

```bash
cat file.txt
```
Prints the contents of a file.

```bash
less file.txt
```
Opens a file in a scrollable viewer. Press q to exit.

```bash
head file.txt
```
Shows the first 10 lines.

```bash
tail file.txt
```
Shows the last 10 lines.

```bash
tail -f /var/log/syslog
```
Follows a log file as new lines are added. The file may not exist on every distribution.

## Finding things

```bash
find . -name "file.txt"
```
Searches for a file by name from the current directory.

```bash
grep "word" file.txt
```
Searches for a word in a file.

```bash
grep -r "word" .
```
Searches recursively through files in the current directory.

## Getting help

```bash
man ls
```
Opens the manual page for a command.

```bash
ls --help
```
Shows available options for ls.

## Notes

- `.` refers to the current directory.
- `..` refers to the parent directory.
- `~` refers to the home directory.
- Use Tab to autocomplete paths and filenames.
- Use the up arrow to cycle through previous commands.
- Be careful with rm. Deleted files generally don't go to a recycle bin.
