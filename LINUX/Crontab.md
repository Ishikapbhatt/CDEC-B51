# What is Crontab?

Crontab (Cron Table) is a Linux utility used to schedule and automate tasks at specific times or intervals. It is commonly used for backups, log rotation, script execution, and system maintenance.

#### Crontab Syntax

**Each line in a crontab file follows this format:**

Minute  Hour  Day  Month  DayOfWeek  Command

![image](https://github.com/user-attachments/assets/1a5417b8-59ba-4ba7-97ba-f64d1fe79f3f)

#### Crontab Special Characters

![image](https://github.com/user-attachments/assets/ef72e03f-408c-4df0-9fa5-35c82049e391)

#### Common Crontab Examples

![image](https://github.com/user-attachments/assets/135ac065-aca6-45c5-95e2-b0b8372a2ae4)

#### Managing Crontab

**Edit the Crontab :**   crontab -e

**View Existing Crontab Jobs :** crontab -l

**Remove All Crontab Jobs :** crontab -r

**Edit Crontab for Another User (Admin Only) :**  sudo crontab -u username -e 
