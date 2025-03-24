# Group Management:

There are 2 categories of groups in the Linux operating system i.e. Primary and Secondary groups. The Primary Group is a group that is automatically generated while creating a user with a unique user ID simultaneously a group with an ID the same as the user ID is created and the user gets added to the group and becomes the first and only member of the group. This group is called the primary group. A secondary group is a group that can be created separately with the help of commands and we can then add users to it by changing the group ID of users.

**CONFIGURATION FILES:**

**/etc/group:** This file stores the groups general information such as redirected password, group ID, group members list.

**Field1:** Group name

**Field2:** Redirected password

**Field3:** Group ID

**Field4:** Group member’s list


**/etc/group-:** This is the back file of the /etc/group

**Field1:** Group name

**Field2:** Encrypted password

**Field3:** Group admin

**Field4:** Group member’s list


**/etc/gshadow:** This file stores the group's password information such as encrypted password, group admin and group members list

**/etc/gshadow-:** This is the back file of the /etc/gshadow


#### Important commands for managing groups

**groupadd:** - To add a secondary Group

**groupmod:** 

**Syntax:**  groupmod  <options>  <arguement>  <existinggroupname>

**OPTIONS:**

**-g=** group id 

**-n=** group name

**-o=** non unique (duplicate)


 **gpasswd** - gpasswd command us used to assign passwords to groups. We can also add members in the group and can create group admin. It repeats on file /etc/gshadow

**Syntax:**  	#gpasswd  <groupname>   assign password to the group
	
  		#gpasswd  <options>  <arguement>  <groupname>

**OPTIONS:**

**-a=** add user in the group

**-d=** delete user from the group

**-r=** remove group password

**-M=** add multiple users in the group but it overwrites to the existing list

**-A=**create group admin

**groupdel:** This command is used to delete group.
