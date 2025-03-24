# Understanding the Linux Command Prompt

The command prompt is a text-based interface where you type commands that the system interprets and executes. It’s where you interact with the shell (typically Bash on many Linux systems), which acts as a command interpreter.

![image](https://github.com/user-attachments/assets/f3d4929b-5764-47d5-99fa-e3dce7537296)

#### **1. Username (user)**
**Purpose:** Displays the username of the person currently logged into the system.

**Example:** If the command prompt is john@hostname:~$, the user logged in is john.

**Significance:** This tells you which user's environment you're working in. If you're the root user, the prompt will change to root@hostname:~#, and the # symbol indicates administrative privileges.

#### **2. Hostname (hostname)**
**Purpose:** Shows the hostname of the machine, which is the name assigned to the system on the network.

**Example:** In user@hostname:~$, hostname could be something like server1, laptop-xyz, etc.

**Significance:** The hostname helps you identify which system you're currently logged into, especially when managing multiple machines or working in a networked environment.

#### **3.  Current Directory (~)**
**Purpose:** Represents the current directory you're in.

**Example:** ~/ represents the home directory of the user, while something like /etc/ represents a system folder.

**Tilde (~):** This is shorthand for the home directory of the current user. For example, /home/user/ is equivalent to ~/ in the prompt.
**Absolute Path:** The full path to the directory you're in, such as /usr/local/bin/.
**Significance:** This shows where you are in the directory structure. If you want to know your full directory path, you can use the pwd (print working directory) command.

#### **4. Prompt Symbol ($ or #)**
**Purpose:** Indicates the type of user account you are using.

$: This symbol means you're logged in as a normal user.
#: If the prompt ends with a #, you are logged in as the root user, which has administrative privileges.
**Example:**

**Regular user:** user@hostname:~$

**Root user:** root@hostname:~#

**Significance:** The symbol shows whether you have administrative privileges, as the root user can perform more critical system

# Introduction to Linux Basic Commands:

#### Basic Commands:

**#pwd** – present working directory

**#clear** – to clear screen  (ctrl+l)

**#exit** – exit from any running utility (Ctrl+d)

**#logout** – logout from any login user

**#history** – display all previously run commands

**#history -c** – to clear all history

**#hostname** – display system/hostname

**#ifconfig** – display IP address of address

**#lsblk** – list block 

**#df –hT** – disk free human readable type

**#reboot** – to restart the system

**#poweroff** – to shut down

**#shutdown**– to shut down

**#shutdown –r** – to restart 

#### SYSTEM COMMANDS:

**#uname –r** – display kernel release version

**#cat /etc/lsb-release** – to display the ubuntu

**#uname –n** – display the node name 

**#uname –o** – display the operating system

**#uname –s** – display the kernel name

**#uname –m** – display machine architecture

**#uname –p** – display the processor architecture

**#lscpu** – display the detail process information

**#cat /proc/cpuinfo** – display the detail process information

**#free** – display memory

**#free –m** – display memory information in MB

**#free –g** – display memory information in GB

**#free –h** – display memory information in human readable

**#dmicode** – display detail information of RAM, HDD, ROM, CPU, etc.

#### Help Commands:

**#man <command_name>** – display the manual page of the command

**#<command_name> --help**  - display all available options of specified command 

**#which <Command_name>** - display the executable file path of specified command 

#### Commands for Navigating the File System:
**ls(list files and directories)** : The ls command is used to list the contents of a directory. It will list down all the files and folders present in the given directory.

**pwd (print working directory)**: At any given moment of time, we will be standing in a certain directory. To get the name of the directory in which we are standing, we can use the pwd command in Linux.

**cd(change directory)** : The cd command can be used to change the working directory. Using the command, you can move from one directory to another.

#### Commands for Manipulating Files:

**touch (create new file):** The touch command can be used to create an empty new file. This command is very useful for many other purposes, but we will discuss the simplest use case of creating a new file.

**mkdir (create new directories)**: The mkdir command is used to create directories. You can use ls command to verify that the new directory is created.

**rm (delete files and directories):** The rm command can be used to delete files and directories. It is very important to note that this command permanently deletes the files and directories. It's almost impossible to recover these files and directories once you have executed rm command on them successfully. 

**cp (copy files and directories):** The cp command is used to copy files and directories from one location to another. Do note that the cp command doesn't do any change to the original files or directories. The original files or directories and their copy both co-exist after running cp command successfully.

**mv (move files and directories): **The mv command can either be used to move files or directories from one location to another or it can be used to rename files or directories. Do note that moving files and copying them are very different. When you move the files or directories, the original copy is lost.

#### Commands for Viewing Files:

**cat:** The most simplest use of cat command is to print the contents of the file on your output screen. This command is very useful and can be used for many other purposes. We will study about other use cases later.

**head: **The head command displays the first 10 lines of the file by default. We can include additional arguments to display as many lines as we want from the top.

**tail:** The tail command displays the last 10 lines of the file by default. We can include additional arguments to display as many lines as we want from the end of the file.

**more:** The more command displays the contents of a file or a command output, displaying one screen at a time in case the file is large (Eg: log files). It also allows forward navigation and limited backward navigation in the file.

**less:** The less command is an improved version of more. It displays the contents of a file or a command output, one page at a time. It allows backward navigation as well as forward navigation in the file and also has search options. We can use arrow keys for advancing backward or forward by one line. For moving forward by one page, press Space and for moving backward by one page, press b on your keyboard. You can go to the beginning and the end of a file instantly.

#### Echo Command in Linux:

The echo command is one of the simplest commands that is used in the shell. This command is equivalent to print in other programming languages.

#### Text Processing Commands:

**grep:** The grep command in its simplest form can be used to search particular words in a text file. It will display all the lines in a file that contains a particular input. The word we want to search is provided as an input to the grep command.

**sed:** The sed command in its simplest form can be used to replace a text in a file.

**sort:** The sort command can be used to sort the input provided to it as an argument. By default, it will sort in increasing order.
