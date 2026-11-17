# Files and directories

A few things worth knowing about how Linux handles files.

## The filesystem

Linux uses a single directory tree starting at `/`, called the root directory.

Some important directories:

| Directory | Purpose |
|---|---|
| `/home` | User home directories |
| `/root` | Root user's home directory |
| `/etc` | System configuration files |
| `/var` | Logs and changing data |
| `/tmp` | Temporary files |
| `/usr` | User applications and shared files |
| `/bin` | Essential user commands |
| `/dev` | Device files |
| `/mnt` | Temporary mount points |
| `/media` | Removable media mount points |

## Hidden files

Files beginning with a dot are hidden by default.

Examples:

- `.bashrc`
- `.profile`
- `.config`
- `.ssh`

To see hidden files:

```bash
ls -la
```

## Absolute and relative paths

An absolute path starts from the root directory.

```bash
/home/user/Documents/file.txt
```

A relative path starts from the current working directory.

```bash
Documents/file.txt
```

## File types

Linux doesn't rely on file extensions to determine file types.

You can check a file using:

```bash
file filename
```

This can identify whether something is a text file, executable, image, archive and so on.

## Disk usage

```bash
du -sh directory
```

Shows the total size of a directory.

```bash
du -h --max-depth=1
```

Shows the size of directories one level below the current directory.

```bash
df -h
```

Shows available and used disk space on mounted filesystems.

## Notes

Linux paths are case-sensitive. `File.txt` and `file.txt` are different filenames.

Most configuration files are stored in `/etc` or in hidden directories inside the user's home directory.
