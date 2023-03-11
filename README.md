## Awesome linux commands

A curated collection of essential Linux commands that are helpful to learn for beginners.

- [1- Navigation commands](#section1) 
- [2- File and directory commands](#section2)
- [3- File viewing and editing commands](#section3)
- [4- System commands](#section4)
- [5- Network commands](#section5)
- [6- User and group commands](#section6)
- [7- Package management commands](#section7)
- [8- Process management commands](#section8)
- [9- System information commands](#section9)
- [10- Security commands](#section10)

<h2 id="section1">1- Navigation commands</h2>

> used to navigate through the file system.

| Command | Description | Example Usage |
|---------|-------------|---------------|
| `cd` | Change directory | `cd /home/user/Documents` |
| `ls` | List contents of directory | `ls -a` |
| `pwd` | Print current working directory | `pwd` |
| `mkdir` | Create new directory | `mkdir new_dir` |
| `rmdir` | Remove directory (if empty) | `rmdir empty_dir` |
| `rm` | Remove file | `rm file.txt` |
| `cp` | Copy file or directory | `cp file.txt new_file.txt` |
| `mv` | Move or rename file or directory | `mv file.txt new_dir/` |


<h2 id="section2">2- File and directory commands</h2>

> used to create, delete, copy, and move files and directories.

| Command | Description | Example Usage |
|---------|-------------|---------------|
| `touch` | Create empty file | `touch file.txt` |
| `cat` | Print contents of file | `cat file.txt` |
| `head` | Print first 10 lines of file | `head file.txt` |
| `tail` | Print last 10 lines of file | `tail file.txt` |
| `less` | View and paginate file contents | `less file.txt` |
| `chmod` | Change file or directory permissions | `chmod 755 file.txt` |
| `chown` | Change file or directory ownership | `chown user:group file.txt` |

<h2 id="section3">3- File viewing and editing commands</h2>

> used to view and edit files.

| Command | Description | Example Usage |
|---------|-------------|---------------|
| `nano` | Basic text editor | `nano file.txt` |
| `vi` or `vim` | Powerful text editor | `vi file.txt` |
| `grep` | Search file for text | `grep "search term" file.txt` |
| `find` | Search for file or directory | `find / -name file.txt` |

<h2 id="section4">4- System commands</h2>

> used to perform system-related tasks such as process management, system monitoring, and service management

| Command | Description | Example Usage |
|---------|-------------|---------------|
| `uname` | Print system information | `uname -a` |
| `whoami` | Print current user | `whoami` |
| `date` | Print current date and time | `date` |
| `shutdown` | Shutdown the system | `shutdown now` |
| `reboot` | Reboot the system | `reboot` |
| `ps` | List running processes | `ps aux` |
| `top` | Display system resource usage | `top` |

<h2 id="section5">5- Network commands</h2>

> used to manage network-related tasks such as connecting to remote servers, checking network status, and managing network interfaces.

| Command | Description | Example Usage |
|---------|-------------|---------------|
| `ping` | Test network connection | `ping google.com` |
| `nslookup` | Look up domain name or IP address | `nslookup google.com` |
| `ifconfig` | Configure network interface | `ifconfig eth0` |
| `ssh` | Secure shell client | `ssh user@hostname` |
| `scp` | Secure copy | `scp file.txt user@hostname:/path/to/destination` |

<h2 id="section6">6- User and group commands</h2>

> used to manage user accounts and groups on the system.

| Command | Description | Example Usage |
|---------|-------------|---------------|
| Command | Description | Example |
| --- | --- | --- |
| addgroup | Create a new group | `addgroup groupname` |
| adduser | Create a new user | `adduser username` |
| delgroup | Remove a group | `delgroup groupname` |
| deluser | Remove a user | `deluser username` |
| groups | Show groups a user belongs to | `groups username` |
| usermod | Modify a user account | `usermod -aG groupname username` |
| groupmod | Modify a group account | `groupmod -n newgroupname groupname` |
| chgrp | Change group ownership of a file | `chgrp groupname filename` |
| id | Display user and group information for the current user | `id` |


<h2 id="section7">7- Package management commands</h2>

> used to manage packages and software on the system.

| Command | Description | Example |
| --- | --- | --- |
| `apt-get install <package>` | Installs a package from the repository | `sudo apt-get install htop` |
| `apt-get remove <package>` | Removes a package | `sudo apt-get remove htop` |
| `apt-get update` | Updates the package list | `sudo apt-get update` |
| `apt-get upgrade` | Upgrades all installed packages to their latest version | `sudo apt-get upgrade` |
| `apt-cache search <package>` | Searches the package list for a package | `apt-cache search php` |
| `dpkg -i <package>.deb` | Installs a package from a .deb file | `sudo dpkg -i google-chrome-stable_current_amd64.deb` |
| `dpkg -r <package>` | Removes a package installed from a .deb file | `sudo dpkg -r google-chrome-stable` |
| `dpkg -l` | Lists all installed packages | `dpkg -l` |

<h2 id="section8">8- Process management commands </h2>

> used to manage processes and their resources.

| Command | Description | Example |
| --- | --- | --- |
| `ps` | Display information about active processes. | `ps aux` |
| `kill` | Send a signal to a process to terminate it. | `kill 1234` |
| `killall` | Send a signal to all processes with a given name to terminate them. | `killall firefox` |
| `top` | Display a real-time view of the processes running on the system. | `top` |
| `htop` | A more advanced version of `top`. | `htop` |
| `nice` | Change the priority of a process. | `nice -n 10 command` |
| `renice` | Change the priority of a running process. | `renice -n 10 1234` |
| `pgrep` | Display the process IDs of processes matching a pattern. | `pgrep firefox` |
| `pkill` | Send a signal to processes matching a pattern to terminate them. | `pkill firefox` |

<h2 id="section9">9- System information commands</h2>

> used to display information about the system, such as hardware information, system uptime, and system version.

| Command | Description | Example |
| ------- | ----------- | ------- |
| df      | Display disk usage statistics | `df -h` |
| lshw    | List hardware configuration | `lshw` |
| lspci   | List PCI devices | `lspci` |
| lsusb   | List USB devices | `lsusb` |
| systemctl | Control the systemd system and service manager | `systemctl status sshd` |
| service | Control system services | `service sshd start` |

<h2>10- Security commands</h2>

> used to manage system security, such as configuring firewall rules, setting file permissions, and managing user authentication.

| Command | Description | Example Usage |
|---------|-------------|---------------|
| `gpg` | Provides encryption and digital signature capabilities for files and emails. | `gpg --encrypt filename` |
| `passwd` | Allows a user to change their own password or an administrator to change the password of another user. | `passwd` or `passwd username` |
| `ssh` | Provides secure, encrypted communication between two untrusted hosts over an insecure network. | `ssh username@remote_host` |
| `sudo` | Allows a user to run a command as another user, typically the superuser. | `sudo command` |
| `ufw` | Uncomplicated Firewall is a user-friendly front-end for managing iptables firewall rules. | `sudo ufw allow ssh` |
| `fail2ban` | Scans log files and bans IPs that show malicious signs. | `sudo fail2ban-client status sshd` |
| `chroot` | Changes the root directory for the current running process and its children. | `sudo chroot /newroot /bin/bash` |
| `chmod` | Changes the file mode (permissions) of a file or directory. | `chmod 755 filename` |
| `chown` | Changes the owner and/or group of a file or directory. | `chown username:groupname filename` |
| `umask` | Sets the default permissions for newly created files and directories. | `umask 022` |
