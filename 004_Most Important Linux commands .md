
# Linux Commands 
Linux commands are instructions or programs that you enter into the terminal or command-line interface of a Linux-based operating system to perform various tasks. These commands allow users to interact with the system, manage files, control processes, configure settings, and perform administrative tasks. Linux commands are typically textual and are executed by typing them into the terminal followed by pressing Enter. They are essential for navigating, managing, and controlling the Linux system efficiently.

Linux/Unix commands are case-sensitive, meaning that uppercase and lowercase letters are treated differently.

---



1. **pwd**:
   - Command: `pwd`
   - Description: Prints the current working directory.
   - Example:
     ```bash
     $ pwd
     /home/user/documents
     ```

2. **whoami**:
   - Command: `whoami`
   - Description: Displays the username of the current user.
   - Example:
     ```bash
     $ whoami
     user
     ```

3. **date**:
   - Command: `date` or `date %D`
   - Description: Shows the system's date and time. Using `%D` formats the date in MM/DD/YY format.
   - Example:
     ```bash
     $ date
     Fri Jun 12 14:30:00 UTC 2024

     $ date %D
     06/12/24
     ```

4. **ls**:
   - Command: `ls` or `ls -lt`
   - Description: Lists files and directories in the current location. Using `-lt` sorts by modification time.
   - Example:
     ```bash
     $ ls
     file1.txt file2.txt directory1

     $ ls -lt
     drwxr-xr-x 2 user user 4096 Jun 12 14:30 directory1
     -rw-r--r-- 1 user user 1024 Jun 10 10:00 file2.txt
     -rw-r--r-- 1 user user 512  Jun 08 08:00 file1.txt
     ```

5. **clear**:
   - Command: `clear`
   - Description: Clears the terminal screen.
   - Example: After executing `clear`, the terminal screen is cleared.

---

# Creating Deleting Editing

6. **cat**:
   - Command: `cat <file>`
   - Description: Displays the content of a file on the terminal.
   - Example:
     ```bash
     $ cat file.txt
     This is the content of the file.
     ```

7. **less**:
   - Command: `less <file>`
   - Description: Allows reading a file and searching for text within it.
   - Example: Type `/` followed by the word to search within the file when in `less`.

8. **more**:
   - Command: `more <file>`
   - Description: Displays the content of a file page by page.
   - Example: Use spacebar to move to the next page and `q` to quit.

9. **touch**:
   - Command: `touch <file_name>`
   - Description: Creates a new empty file with the specified name.
   - Example:
     ```bash
     $ touch new_file.txt
     ```

10. **rm**:
    - Command: `rm <file_name>`
    - Description: Removes or deletes a file.
    - Example:
      ```bash
      $ rm old_file.txt
      ```

11. **vi / nano** (Edit a file):
    - Command: `vi <file_name>` or `nano <file_name>`
    - Description: Opens the specified file in the Vi or Nano text editors for editing.
    - Example:
      ```bash
      $ vi example.txt
      ```

12. **mkdir** (Create a directory/folder):
    - Command: `mkdir <directory_name>`
    - Description: Creates a new directory with the specified name.
    - Example:
      ```bash
      $ mkdir new_directory
      ```

13. **rmdir / rm -rf** (Delete a directory/folder):
    - Command: `rmdir <directory_name>` or `rm -rf <directory_name>`
    - Description: Removes or deletes the specified directory. Use `rm -rf` for directories with content.
    - Example:
      ```bash
      $ rmdir old_directory
      $ rm -rf directory_with_files
      ```

14. **cd** (Change path or move to another folder):
    - Command: `cd /path/to/folder` or `cd ..` (moves up one level)
    - Description: Changes the current directory to the specified path or moves up one level in the directory hierarchy.
    - Example:
      ```bash
      $ cd /home/user/documents
      $ cd ..
      ```

15. **cp** (Copy and paste a file):
    - Command: `cp <file> /destination/path`
    - Description: Copies the specified file to the destination path.
    - Example:
      ```bash
      $ cp example.txt /backup/documents
      ```

16. **cp** (Copy content of a file to another file):
    - Command: `cp fileA fileB`
    - Description: Copies the content of fileA to fileB.
    - Example:
      ```bash
      $ cp source_file.txt destination_file.txt
      ```

17. **mv** (Cut - paste a file):
    - Command: `mv <file> /destination/path` or `mv fileA fileNewName`
    - Description: Moves (cuts) the specified file to the destination path or renames the file.
    - Example:
      ```bash
      $ mv example.txt /new_location/
      $ mv old_name.txt new_name.txt
      ```

18. **head** (Read or display top lines from a file):
    - Command: `head -5 file`
    - Description: Displays the first 5 lines of the specified file.
    - Example:
      ```bash
      $ head -5 data_file.txt
      ```

19. **tail** (Read or display bottom lines from a file):
    - Command: `tail -5 file`
    - Description: Displays the last 5 lines of the specified file.
    - Example:
      ```bash
      $ tail -5 data_file.txt
      ```

20. **sort** (Sort the content of a file):
    - Command: `sort file` or `sort -r file` (reverse order)
    - Description: Sorts the content of the file in ascending or descending order.
    - Example:
      ```bash
      $ sort names.txt
      $ sort -r numbers.txt
      ```

21. **sort | uniq** (Display unique content from a file):
    - Command: `sort file | uniq`
    - Description: Displays only unique lines from the sorted content of the file.
    - Example:
      ```bash
      $ sort data.txt | uniq
      ```

22. **split** (Split a file into multiple files):
    - Command: `split -l 3 file` (splits into files with 3 lines each)
    - Description: Splits the file into multiple smaller files based on the specified number of lines.
    - Example:
      ```bash
      $ split -l 3 big_file.txt
      ```

23. **grep** (Search a word and display matching content):
    - Command: `grep "word" file`
    - Description: Searches for the specified word in the file and displays matching lines.
    - Example:
      ```bash
      $ grep "error" log_file.txt
      ```

24. **egrep** (Search multiple words and display matching content):
    - Command: `egrep "word1|word2" file`
    - Description: Searches for multiple words (using OR) in the file and displays matching lines.
    - Example:
      ```bash
      $ egrep "error|warning" log_file.txt
      ```

25. **ls / touch** (Using wildcards in Linux):
    - Command: `ls file*` or `touch file{1..5}`
    - Description: Uses wildcards (`*`, `{}`, `[]`) to match patterns or generate multiple file names.
    - Example:
      ```bash
      $ ls backup*.txt
      $ touch file{1..5}.txt
      ```

26. **shuf** (Shuffle content of file):
    - Command: `shuf file`
    - Description: Randomly shuffles the lines in the file.
    - Example:
      ```bash
      $ shuf names.txt
      ```

27. **wc** (Count number of lines in a file):
    - Command: `wc -l file`
    - Description: Counts and displays the number of lines in the file.
    - Example:
      ```bash
      $ wc -l data.txt
      ```

28. **cmp** (Check if two files are identical):
    - Command: `cmp fileA fileB`
    - Description: Compares two files byte by byte and displays the first differing byte.
    - Example:
      ```bash
      $ cmp original.txt backup.txt
      ```

29. **diff** (Compare and display difference between two files):
    - Command: `diff -u fileA fileB`
    - Description: Compares two files line by line and displays the differences in a unified format.
    - Example:
      ```bash
      $ diff -u old_file.txt new_file.txt
      ```

30. **find** (Find a file in Linux):
    - Command: `find /path/ -name <file>`
    - Description: Searches for a file with the specified name in the specified path.
    - Example:
      ```bash
      $ find /home/user/documents -name example.txt
      ```

31. **updatedb / locate** (Update and locate a file):
    - Command: `updatedb` (updates the locate database) and `locate <file>`
    - Description: Updates the database used by `locate` command to find files quickly.
    - Example:
      ```bash
      $ updatedb
      $ locate example.txt
      ```

---

# Utility commands in Linux:

32. **history** (Display previously used commands):
    - Command: `history`
    - Description: Displays a list of previously used commands in the terminal session.
    - Example:
      ```bash
      $ history
      ```

33. **help** (Check syntax and options available for a command):
    - Command: `help`
    - Description: Provides information about built-in shell commands.
    - Example:
      ```bash
      $ help cd
      ```

34. **man** (Read or get more info about a command):
    - Command: `man <command>`
    - Description: Displays the manual pages for the specified command, providing detailed information and usage examples.
    - Example:
      ```bash
      $ man ls
      ```

35. **which** (Check which executable is used for a command):
    - Command: `which <command>`
    - Description: Displays the path of the executable file that will be executed when the command is run.
    - Example:
      ```bash
      $ which python
      ```

36. **bc** (Use calculator in Linux):
    - Command: `bc`
    - Description: Launches the calculator utility for performing arithmetic calculations.
    - Example:
      ```bash
      $ bc
      ```

37. **cal** (Check calendar of last year in Linux):
    - Command: `cal -3`
    - Description: Displays the calendar of the previous, current, and next month or year.
    - Example:
      ```bash
      $ cal -3
      ```

38. **uptime** (Check how long server has been running):
    - Command: `uptime`
    - Description: Displays information about how long the system has been running.
    - Example:
      ```bash
      $ uptime
      ```

39. **script** (Record your activity on terminal in a file):
    - Command: `script <filename>`
    - Description: Starts a script session that records all terminal input and output to the specified file.
    - Example:
      ```bash
      $ script session.log
      ```

40. **alias** (Create an alias for a command):
    - Command: `alias l="ls -ltr"`
    - Description: Creates a shortcut (alias) for a longer command. In this example, `l` is aliased to `ls -ltr`.
    - Example:
      ```bash
      $ alias l="ls -ltr"
      ```

---

#  zip and unzip commands in Linux:

41. **gzip -k file** (Compress a file in Linux):
    - Command: `gzip -k <file>`
    - Description: Compresses the specified file and keeps the original file (`-k` option).
    - Example:
      ```bash
      $ gzip -k myfile.txt
      ```

42. **gzip -d file** / **gunzip file** (Decompress a file in Linux):
    - Commands: `gzip -d <file>` / `gunzip <file>`
    - Description: Decompresses the specified gzip-compressed file.
    - Examples:
      ```bash
      $ gzip -d myfile.txt.gz
      $ gunzip myfile.txt.gz
      ```

43. **tar -czf myfiles.tar.gz myfiles/** (Compress a folder in Linux):
    - Command: `tar -czf <output-file.tar.gz> <folder-to-compress>`
    - Description: Creates a compressed tarball (.tar.gz) of the specified folder.
    - Example:
      ```bash
      $ tar -czf myfiles.tar.gz myfiles/
      ```

44. **tar -xzf myfiles.tar.gz** (Decompress a folder in Linux):
    - Command: `tar -xzf <compressed-file.tar.gz>`
    - Description: Extracts the contents of a compressed tarball (.tar.gz) into the current directory.
    - Example:
      ```bash
      $ tar -xzf myfiles.tar.gz
      ```

45. **zip myfiles.zip file1 file2** (Compress multiple files into one zipped file in Linux):
    - Command: `zip <output-zip-file> <file1> <file2> ...`
    - Description: Creates a zipped archive containing multiple specified files.
    - Example:
      ```bash
      $ zip myfiles.zip file1.txt file2.txt
      ```

46. **unzip -l myfiles.zip** (List files in a zipped file in Linux):
    - Command: `unzip -l <zip-file>`
    - Description: Lists the files and directories contained within the specified zipped file.
    - Example:
      ```bash
      $ unzip -l myfiles.zip
      ```

---

# Downloading Files from Internet

47. **wget URL** (Download a file from the internet using wget):
   - Command: `wget <URL>`
   - Description: Downloads a file from the specified URL and saves it in the current directory.
   - Example: 
     ```bash
     $ wget https://example.com/file.zip
     ```

48. **wget -O output-file.txt URL** (Download a file and save with a specific name using wget):
   - Command: `wget -O <output-file> <URL>`
   - Description: Downloads a file from the specified URL and saves it with the specified name.
   - Example:
     ```bash
     $ wget -O myfile.zip https://example.com/file.zip
     ```

49. **curl http://numbersapi.com/random** (Call an API using curl on Linux):
   - Command: `curl <API_URL>`
   - Description: Calls the specified API URL using curl and retrieves the response.
   - Example:
     ```bash
     $ curl http://numbersapi.com/random
     ```

50. **apt or yum/dnf** (Install an application using package managers on Linux):
   - Commands:
     - `apt install <package-name>` (APT)
     - `yum install <package-name>` or `dnf install <package-name>` (YUM/DNF)
   - Description: Installs the specified package using the respective package manager.
   - Example:
     ```bash
     $ apt install nginx
     $ yum install httpd
     ```

51. **rpm -qa | grep app** / **dnf list installed** (Check if an application is installed on Linux):
   - Commands:
     - `rpm -qa | grep <app-name>` (RPM)
     - `dnf list installed | grep <app-name>` (DNF)
   - Description: Checks if the specified application is installed using RPM or DNF package managers.
   - Example:
     ```bash
     $ rpm -qa | grep mysql
     $ dnf list installed | grep nginx
     ```

52. **apt search <package-name>** / **yum/dnf list available** (List available packages to install on Linux):
   - Commands:
     - `apt search <package-name>` (APT)
     - `yum list available <package-name>` or `dnf list available <package-name>` (YUM/DNF)
   - Description: Lists available packages matching the specified name using the respective package manager.
   - Example:
     ```bash
     $ apt search nodejs
     $ yum list available php
     ```

53. **systemctl start/stop service-name** (Start/stop a service on Linux):
   - Commands: `systemctl start <service-name>` / `systemctl stop <service-name>`
   - Description: Starts or stops the specified service using systemctl.
   - Example:
     ```bash
     $ systemctl start nginx
     $ systemctl stop apache2
     ```

54. **systemctl list-units --type=service --all** (List all services on Linux):
   - Command: `systemctl list-units --type=service --all`
   - Description: Lists all services available on the system using systemctl.
   - Example:
     ```bash
     $ systemctl list-units --type=service --all
     ```

55. **printenv** (List all existing environment variables on Linux):
   - Command: `printenv`
   - Description: Prints all existing environment variables and their values.
   - Example:
     ```bash
     $ printenv
     ```

56. **export JAVA_HOME="/usr/lib/jvm/java-v" / export PATH=$JAVA_HOME/bin:$PATH** (Add a new environment variable temporarily/permanently on Linux):
   - Commands: 
     - `export <variable-name>=<value>` (Temporary)
     - Edit `~/.bashrc` or `~/.bash_profile` and add `export <variable-name>=<value>` (Permanent)
   - Description: Adds a new environment variable temporarily or permanently.
   - Example (temporary):
     ```bash
     $ export JAVA_HOME="/usr/lib/jvm/java-v"
     $ export PATH=$JAVA_HOME/bin:$PATH
     ```

57. **awk -F , '{print $2}' file.csv** (Print a specific column from a CSV file in Linux):
   - Command: `awk -F , '{print $<column-number>}' <file.csv>`
   - Description: Prints the specified column (based on column number) from a CSV file using awk.
   - Example:
     ```bash
     $ awk -F , '{print $2}' data.csv
     ```

58. **cut -c1-2 file.txt** (Display starting two characters of all lines in Linux):
   - Command: `cut -c<start>-<end> <file.txt>`
   - Description: Displays the specified range of characters from each line of the file.
   - Example:
     ```bash
     $ cut -c1-2 myfile.txt
     ```

59. **sed -n '5p' file.txt** (Display a specific line from a file in Linux):
   - Command: `sed -n '<line-number>p' <file.txt>`
   - Description: Displays the specified line number from the file using sed.
   - Example:
     ```bash
     $ sed -n '5p' myfile.txt
     ```

60. **sed -n 's/from/to/g' file.txt** (Replace a specific word within a file in Linux):
   - Command: `sed -n 's/<from>/<to>/g' <file.txt>`
   - Description: Replaces occurrences of `<from>` with `<to>` globally in the file using sed.
   - Example:
     ```bash
     $ sed -n 's/old/new/g' myfile.txt
     ```

61. **tr [:lower:] [:upper:] <file.txt** / **tr [:punct:] Z <file.txt** / **tr [:digit:] Z <file.txt** (Convert content to uppercase/lowercase/digit substitution within a file in Linux):
   - Commands:
     - `tr [:lower:] [:upper:] <file.txt>` (Uppercase)
     - `tr [:punct:] Z <file.txt>` (Replace punctuation with 'Z')
     - `tr [:digit:] Z <file.txt>` (Replace digits with 'Z')
   - Description: Converts text to uppercase/lowercase or replaces characters using tr command.
   - Examples:
     ```bash
     $ tr [:lower:] [:upper:] myfile.txt
     $ tr [:punct:] Z myfile.txt
     $ tr [:digit:] Z myfile.txt
     ```

62. **truncate -s 100M file.txt** (Extend or shrink size of a file in Linux):
   - Command: `truncate -s <size> <file.txt>`
   - Description: Changes the size of the specified file to the specified size.
   - Example:
     ```bash
     $ truncate -s 100M myfile.txt
     ```


63. **echo "ABCDE" | fold -w1** (Display text in vertical lines in Linux):
   - Command: `echo "<text>" | fold -w1`
   - Description: Displays the specified text in vertical lines, with each character on a separate line.
   - Example:
     ```bash
     $ echo "ABCDE" | fold -w1
     ```

64. **su <username>** (Change user or login as a different user in Linux):
   - Command: `su <username>`
   - Description: Switches to the specified user account, requiring the user's password.
   - Example:
     ```bash
     $ su john_doe
     ```

65. **exit** (Exit as the current user or close the terminal in Linux):
   - Command: `exit`
   - Description: Closes the current terminal session or exits from the current user session if using the `su` command.
   - Example:
     ```bash
     $ exit
     ```

66. **sudo yum install httpd** (Install an application using sudo and yum in Linux):
   - Command: `sudo yum install <package-name>`
   - Description: Installs the specified package using the yum package manager with administrative privileges.
   - Example:
     ```bash
     $ sudo yum install httpd
     ```

---

# Access Remote Servers

Here are the notes for the specified commands:

67. **ssh user@hostname** (Access remote Linux server using SSH):
   - Command: `ssh <username>@<hostname>`
   - Description: Establishes a secure shell (SSH) connection to a remote Linux server using the specified username and hostname. Requires the user's password or SSH key for authentication.
   - Example:
     ```bash
     $ ssh john_doe@example.com
     ```

68. **scp file user@hostname:/tmp/** (Copy files to a remote server using SCP):
   - Command: `scp <file> <username>@<hostname>:/<remote-directory>/`
   - Description: Copies the specified file to a remote server using the SCP (Secure Copy) protocol. Requires the destination username, hostname, and directory on the remote server.
   - Example:
     ```bash
     $ scp myfile.txt john_doe@example.com:/tmp/
     ```

---

#### Working with Permissions


69. **ls -ltr** (Check permissions of a file):
   - Command: `ls -ltr`
   - Description: Lists files and their details, including permissions, ownership, and modification time, in long format with the newest files at the bottom.
   - Example:
     ```bash
     $ ls -ltr
     ```

70. **chmod a+rwx file.txt** (Modify permissions of a file):
   - Command: `chmod <permissions> <file>`
   - Description: Changes the permissions of a file. The permissions can be specified for user (u), group (g), other (o), or all (a) using symbols (+ for adding permissions, - for removing 
     permissions, = for setting exact permissions), followed by r (read), w (write), and x (execute) permissions.
   - Example:
     ```bash
     $ chmod a+rwx file.txt
     ```

71. **chown root file.txt** (Change ownership of a file):
   - Command: `chown <new-owner> <file>`
   - Description: Changes the ownership of a file to the specified user or group. The new owner can be specified by username or group name.
   - Example:
     ```bash
     $ chown root file.txt
     ```

72. **chgrp paul file.txt** (Change group ownership of a file):
   - Command: `chgrp <new-group> <file>`
   - Description: Changes the group ownership of a file to the specified group. The new group can be specified by group name.
   - Example:
     ```bash
     $ chgrp paul file.txt
     ```


---

# Memory Info

Here are the notes for the specified commands:

73. **free** (Check free RAM space):
   - Command: `free`
   - Description: Displays information about total, used, and free memory (RAM) in the system, including buffers and cache memory.
   - Example:
     ```bash
     $ free
     ```

74. **top** (Check % Memory and CPU Utilization):
   - Command: `top`
   - Description: Displays real-time information about system processes, including CPU and memory utilization, sorted by various criteria like CPU usage.
   - Example:
     ```bash
     $ top
     ```

75. **du** (Check disk utilization):
   - Command: `du`
   - Description: Displays disk usage of files and directories in the current directory or specified path, showing the disk space consumed by each file and directory.
   - Example:
     ```bash
     $ du
     ```

76. **df** (Check disk space and utilization):
   - Command: `df`
   - Description: Displays disk space usage and information about mounted filesystems, including total, used, and available space, as well as the percentage of disk space used.
   - Example:
     ```bash
     $ df
     ```

---

# System INFO


77. **hostname** (Check hostname of your Linux server):
   - Command: `hostname`
   - Description: Displays the hostname of the system, which is the name assigned to the server or machine.
   - Example:
     ```bash
     $ hostname
     ```

78. **lscpu** (Check CPU/core/thread info of your Linux server):
   - Command: `lscpu`
   - Description: Displays detailed information about the CPU architecture, cores, threads, and other CPU-related information.
   - Example:
     ```bash
     $ lscpu
     ```

79. **arch** (Check type of architecture of your Linux server):
   - Command: `arch`
   - Description: Displays the type of architecture of the system, such as x86_64, arm, etc., indicating the processor architecture.
   - Example:
     ```bash
     $ arch
     ```

80. **lsblk** (See list of storage devices, disk partitions on your Linux server):
   - Command: `lsblk`
   - Description: Lists information about block devices, including storage devices (like hard drives, SSDs) and their partitions, if any.
   - Example:
     ```bash
     $ lsblk
     ```

81. **uname -a** (Display system information including kernel version):
   - Command: `uname -a`
   - Description: Prints detailed system information, including the kernel name, version, architecture, hostname, and more.
   - Example:
     ```bash
     $ uname -a
     ```

---

# Process Management


82. **ps -ef | grep java** (Check if a process (java) is running or not):
   - Command: `ps -ef | grep java`
   - Description: Lists all processes and filters for those containing the keyword "java". It helps check if a Java process is running.
   - Example:
     ```bash
     $ ps -ef | grep java
     ```

83. **pgrep chron** (Get PID of a process):
   - Command: `pgrep chron`
   - Description: Retrieves the Process ID (PID) of a process based on its name, in this case, "chron".
   - Example:
     ```bash
     $ pgrep chron
     ```

84. **kill -9 PID** (Stop a process by PID):
   - Command: `kill -9 PID`
   - Description: Sends a SIGKILL signal (signal 9) to the process with the specified PID, forcefully terminating it.
   - Example:
     ```bash
     $ kill -9 1234
     ```

85. **pkill httpd** (Stop a process by its name):
   - Command: `pkill httpd`
   - Description: Terminates all processes with the name "httpd", effectively stopping the Apache HTTP Server.
   - Example:
     ```bash
     $ pkill httpd
     ```

86. **jobs** (See all active jobs):
   - Command: `jobs`
   - Description: Lists all jobs (background and suspended) associated with the current shell session.
   - Example:
     ```bash
     $ jobs
     ```

87. **bg** (Resume a job in background):
   - Command: `bg`
   - Description: Resumes a suspended job in the background, allowing it to continue executing.
   - Example:
     ```bash
     $ bg
     ```

88. **fg** (Resume a job in foreground):
   - Command: `fg`
   - Description: Brings a background job to the foreground, making it the active job.
   - Example:
     ```bash
     $ fg
     ```

89. **nohup ./script >/dev/null &** (Run a script in background with no hangup):
   - Command: `nohup ./script >/dev/null &`
   - Description: Executes a script called "script" in the background, ignoring hangup signals (SIGHUP), and redirects output to /dev/null to discard it.
   - Example:
     ```bash
     $ nohup ./script >/dev/null &
     ```

---

# Networking Info


90. **ifconfig** (Check IP of your machine):
   - Command: `ifconfig`
   - Description: Displays network interface configuration, including IP addresses assigned to each interface.
   - Example:
     ```bash
     $ ifconfig
     ```

91. **ping www.google.com** (Check if a server or website is accessible):
   - Command: `ping www.google.com`
   - Description: Sends ICMP echo requests to the specified domain (e.g., www.google.com) to check if it's reachable and measure round-trip time.
   - Example:
     ```bash
     $ ping www.google.com
     ```

92. **telnet IP Port** (Check if an IP:PORT is accessible and open):
   - Command: `telnet IP Port`
   - Description: Attempts to establish a TCP connection to the specified IP address and port to check if it's open and accessible.
   - Example:
     ```bash
     $ telnet 192.168.1.1 80
     ```

93. **netstat -putan | grep 80** (Check if a port is open on our server):
   - Command: `netstat -putan | grep 80`
   - Description: Lists all network connections, filtering for those using port 80. It helps check if port 80 is open on the server.
   - Example:
     ```bash
     $ netstat -putan | grep 80
     ```

94. **traceroute** (Check all hops in network path to reach a website):
   - Command: `traceroute`
   - Description: Traces the route packets take from your system to a specified destination, showing all intermediate hops.
   - Example:
     ```bash
     $ traceroute www.google.com
     ```

95. **reboot** (Restart our Linux server):
   - Command: `reboot`
   - Description: Initiates a system reboot, shutting down and restarting the server.
   - Example:
     ```bash
     $ reboot
     ```

96. **shutdown** (Shut down our Linux server):
   - Command: `shutdown`
   - Description: Initiates a system shutdown, powering off the server.
   - Example:
     ```bash
     $ shutdown now
     ```

---

# User Creation


97. **useradd** (Create a new user on our Linux server):
   - Command: `useradd username`
   - Description: Adds a new user to the system with the specified username. Additional options can be used to set user properties like home directory, shell, etc.
   - Example:
     ```bash
     $ useradd john
     ```

98. **passwd** (Change password for the user):
   - Command: `passwd username`
   - Description: Allows the user or root to change the password for the specified user.
   - Example:
     ```bash
     $ passwd john
     ```

99. **groupadd** (Create a new group on our Linux server):
   - Command: `groupadd groupname`
   - Description: Creates a new group with the specified groupname.
   - Example:
     ```bash
     $ groupadd developers
     ```

100. **id user** (Check UserID or GroupID of a user):
    - Command: `id username`
    - Description: Displays user information, including user ID (UID), group ID (GID), and group membership.
    - Example:
      ```bash
      $ id john
      ```

101. **userdel <user>** (Delete a user):
    - Command: `userdel username`
    - Description: Deletes the specified user from the system, removing associated files depending on options used.
    - Example:
      ```bash
      $ userdel john
      ```

102. **groupdel <group>** (Delete a group):
    - Command: `groupdel groupname`
    - Description: Deletes the specified group from the system.
    - Example:
      ```bash
      $ groupdel developers
      ```
---


