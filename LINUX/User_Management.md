# User Management in Linux

A user is an entity, in a Linux operating system, that can manipulate files and perform several other operations. Each user is assigned an ID that is unique for each user in the operating system. In this post, we will learn about users and commands which are used to get information about the users. After installation of the operating system, the ID 0 is assigned to the root user and the IDs 1 to 999 (both inclusive) are assigned to the system users and hence the ids for local user begins from 1000 onwards. 

**Note:** In a single directory, we can create 60,000 users.

**CONFIGURATION FILES:**

**/etc/passwd:** This files stores the users general information such as user ID, Group ID, User’s home directory, login shell, comment, etc.

**Field1:** User name

**Field2:** Redirected password

**Field3:** User ID

**Field :** Group ID

**Field 5:** Comment

**Field 6:** User’s home directory

**Field 7:** User’s login shell


**/etc/passwd-:** This is the back file of the /etc/passwd

**Field1:** User name

**Field2:** Encrypted password

**Field3:** Last password change day

**Field4:** Minimum password age

**Field5:** Maximum password age

**Field6:** Warming period

**Field7:** Inactive password

**Field8**: Account Expiry

**Field9:** Future reserved



**/etc/shadow**: This files stores the User’s password information such as encrypted password, last password change day, minimum password age, maximum password age, password, inactive, account expiry, etc

**/etc/shadow-**: This is the back file of the /etc/shadow

**/etc/default/useradd:** This is default configuration file for useradd command 

**/etc/login.defs:** This is main configuration file for user administration, group administration and password policies. If this file corrupts you can not perform user administration, group administration and password policies.

**/etc/bashrc:** Global login program file

**/etc/skel:** Skeleton Directory

	  .bashrc = local login program file 
	  . bash_profile = local user’s profile program file
	  . bash_logout = local user’s logout program file

#### Important commands for managing users:

**id command** - id command can be used to find the uid and gid associated with an user. It also lists down the groups to which the user belongs to.

**useradd**: The useradd command adds a new user in Linux. We will create a new user shivam. We will also verify that the user has been created by tailing the /etc/passwd file. The uid and gid are 1000 for the newly created user. The home directory assigned to the user is /home/shivam and the login shell assigned is /bin/bash. Do note that the user home directory and login shell can be modified later on.



**passwd**:  The passwd command is used to create or modify passwords for a user. In the above examples, we have not assigned any password for users shivam or amit while creating them. !! in an account entry in shadow means the account of an user has been created, but not yet given a password.

**Syntax:**
	
 #passwd  to change self passwd

 #passwd <username>  assign password to the user

 $passwd  to change self password (local user)

 #passwd <options>  <argument>  <username>

**OPTIONS:**

**-n=** minimum password age

**-x=** maximum password age

**-w=** warning period

**-i=** inactive passwd

**-e=** immediate expiry of account

**-l=** lock password

**-u=** unlock password

**-s=** status


**usermod**: The usermod command is used to modify the attributes of an user like the home directory or the shell.

**Syntax:** #usermod <options>  <argument>  <username>

**OPTIONS:**

**-u=** user id uid

**-g=** group id gid

**-c=** comment

**-d=** home directory

**-s=** login shell

**-G=** group assign

**-e=** account expiry

**-f=** password inactive

**-N=** do not create user’s primary group

**-r=** system user

**-o=** non unique

**-p=** set password

**-l=** login shell

**-L=** lock user account

**-U=** Unlock user account


**chage** - chage command is used to change the password policies of users. Password policies such as minimum password age, maximum password age, password inactive, warning period, account expiry, etc. chage is the acronym of change age


**OPTIONS:**

**-l=** list the password policies

**-d=** last password change day

**-m=** Minimum password age

**-M=** Maximum password age

**-W=** Warning period

**-I=** Inactive password period

**-E=** Account expiry


**userdel:** The userdel command is used to remove a user on Linux. Once we remove a user, all the information related to that user will be removed.
