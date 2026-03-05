# Linux Lab – File Navigation, Permissions, and Privilege Escalation

## Objective
Gain familiarity with basic Linux command-line operations including file navigation, permission management, and administrative privilege escalation.

## Environment
- Ubuntu 22.04 ARM64
- Virtual machine running in UTM on macOS (Apple Silicon)
- Terminal interface used for command execution

---

## File System Navigation

The following commands were used to explore and navigate the Linux file system.

### Commands Used

pwd
ls
ls -la
cd

### Actions Performed

- Verified current working directory using `pwd`
- Listed files and folders using `ls`
- Displayed hidden files and permissions using `ls -la`
- Navigated directories including `/`, `/home`, and the current user's home directory using `cd`

This exercise demonstrated the hierarchical structure of the Linux file system.

---

## File Creation and Deletion

Basic file and directory management commands were practiced.

### Commands Used

touch labfile.txt
mkdir labfolder
ls
rm labfile.txt
rmdir labfolder

### Actions Performed

- Created a test file using `touch`
- Created a directory using `mkdir`
- Verified creation using `ls`
- Removed the file using `rm`
- Removed the directory using `rmdir`

This demonstrates basic file system management through the command line.

---

## File Permission Management

Linux file permissions were inspected and modified.

### View Permissions

Command used:

ls -l

Example output:

-rw-r--r--

### Permission Structure

Linux permissions follow this model:

Owner | Group | Others

Example breakdown:

-rw-r--r--

- Owner: read/write
- Group: read
- Others: read

---

### Modify File Permissions

Command used:

chmod 600 securefile.txt

After modification:

-rw-------

This restricts file access so that only the file owner can read or write the file.

This demonstrates secure file access management using the `chmod` command.

---

## Privilege Escalation with sudo

Linux administrative actions require elevated privileges.

### Attempted Software Installation Without Privileges

Command used:

apt install htop

Result: Permission denied due to insufficient privileges.

---

### Install Package Using Elevated Privileges

Commands used:

sudo apt update
sudo apt install htop

The `sudo` command temporarily grants administrative permissions allowing the installation to complete.

---

## Verification

The installed package was verified using:

htop

The system monitoring tool launched successfully, confirming the installation was completed using elevated privileges.

---

## Simulated Help Desk Scenario

### Issue
User attempted to install software but received a permission denied error.

### Troubleshooting Steps
1. Reviewed the error message from the terminal.
2. Determined that the operation required administrative privileges.
3. Used `sudo` to execute the command with elevated permissions.
4. Successfully installed the application.

### Resolution
Software installation was completed using elevated privileges through the `sudo` command.

---

## Skills Demonstrated

- Linux terminal navigation
- File system structure awareness
- File and directory management
- File permission management using `chmod`
- Privilege escalation using `sudo`
- Linux package installation using `apt`
- Command-line troubleshooting
