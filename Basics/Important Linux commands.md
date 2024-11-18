# Essential Linux Commands

## **1. `ls`**
List directory contents.
- Example: `ls -l` (detailed listing)

## **2. `cd`**
Change directory.
- Example: `cd /home` (navigate to `/home`)

## **3. `pwd`**
Print working directory.
- Example: `pwd` (shows the current directory)

## **4. `cp`**
Copy files or directories.
- Example: `cp source.txt destination.txt`

## **5. `mv`**
Move or rename files or directories.
- Example: `mv oldname.txt newname.txt`

## **6. `rm`**
Remove files or directories.
- Example: `rm file.txt` (removes a file)
- For directories: `rm -r directory_name`

## **7. `mkdir`**
Create directories.
- Example: `mkdir new_directory`

## **8. `rmdir`**
Remove empty directories.
- Example: `rmdir empty_directory`

## **9. `touch`**
Create an empty file or update the timestamp of an existing file.
- Example: `touch newfile.txt`

## **10. `cat`**
Concatenate and display file content.
- Example: `cat file.txt`

## **11. `man`**
Show manual pages for commands.
- Example: `man ls` (opens the manual for `ls`)

## **12. `chmod`**
Change file permissions.
- Example: `chmod 755 script.sh`

## **13. `chown`**
Change file owner.
- Example: `chown user:group file.txt`

## **14. `sudo`**
Run a command as superuser (admin).
- Example: `sudo apt-get update`

## **15. `apt-get`**
Install, update, and remove packages (Debian-based systems).
- Example: `sudo apt-get install package_name`

## **16. `ps`**
Display current processes.
- Example: `ps aux`

## **17. `kill`**
Terminate a process by PID.
- Example: `kill 1234` (where 1234 is the process ID)

## **18. `grep`**
Search for a specific pattern in files.
- Example: `grep "text" file.txt`

## **19. `find`**
Search for files in a directory hierarchy.
- Example: `find / -name "filename"`

## **20. `top`**
Display real-time system processes.

## **21. `df`**
Show disk usage of file systems.
- Example: `df -h` (human-readable format)

## **22. `du`**
Show disk usage of files and directories.
- Example: `du -sh` (summary, human-readable)

## **23. `echo`**
Display a line of text or a variable.
- Example: `echo "Hello, World!"`

## **24. `tar`**
Archive files.
- Example: `tar -czvf archive.tar.gz /path/to/dir`

## **25. `zip/unzip`**
Compress/uncompress files.
- Example: `zip archive.zip file1 file2`

## **26. `scp`**
Securely copy files between computers.
- Example: `scp file.txt user@remote:/path`

## **27. `ssh`**
Secure Shell for remote login.
- Example: `ssh user@hostname`

## **28. `wget`**
Download files from the web.
- Example: `wget http://example.com/file.zip`

## **29. `curl`**
Transfer data from or to a server.
- Example: `curl -O http://example.com/file.txt`

## **30. `head`**
Display the first part of a file.
- Example: `head -n 10 file.txt`

## **31. `tail`**
Display the last part of a file.
- Example: `tail -n 10 file.txt`

## **32. `history`**
Show command history.

## **33. `alias`**
Create a shortcut for commands.
- Example: `alias ll='ls -la'`

## **34. `ln`**
Create symbolic/hard links.
- Example: `ln -s /path/to/file link_name`

## **35. `ping`**
Test network connectivity.

## **36. `whoami`**
Display the current user.

## **37. `useradd`**
Add a new user.
- Example: `sudo useradd username`

## **38. `usermod`**
Modify a user account.
- Example: `sudo usermod -aG groupname username`

## **39. `passwd`**
Change a user’s password.
- Example: `passwd username`

## **40. `df -Th`**
Display file system type and disk space usage.
- Example: `df -Th`

## **41. `uname -r`**
Show kernel version.
- Example: `uname -r`

## **42. `uptime`**
Show how long the system has been running.
- Example: `uptime`

## **43. `free`**
Display memory usage.
- Example: `free -h`

## **44. `locate`**
Find files by name.
- Example: `locate filename`

## **45. `nano`**
Text editor in the terminal.
- Example: `nano file.txt`

## **46. `vi`**
Another text editor in the terminal.
- Example: `vi file.txt`

## **47. `env`**
Display environment variables.

## **48. `export`**
Set or export an environment variable.
- Example: `export PATH=$PATH:/newpath`

## **49. `crontab`**
Schedule a task.
- Example: `crontab -e` (edit crontab)

## **50. `service`**
Control services (start, stop, restart).
- Example: `sudo service apache2 restart`
