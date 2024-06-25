# Ghost-Script.2024

This script is can only be used for data migration between old server to new server in a Linux based platform. Any modification of the code without the permission of the author is against their right of ownership. For more information please read the terms and conditions mentioned in the license file. The Ghost Script 2024 is always subject to be update annually for any additional updates that helps to improve our server performance so don’t forget to ask the author for the updated version.

Getting Started
Assuming that the server was already configured and cleaned for unnecessarily files. You may now follow step by step for Data Migration.
Step 1:
 Mount your flash drive manually. Sometimes there is a red hat version that perform auto mount. This is common in some flash drive vendors. If your flash drive perform auto mount upon inserting the drive just unmount and do mounting manually. In order to mount your flash drive manually, do this command.

mount /dev/sdb1 /media ----------This mount command is for the main server or the 192.168.0.10 server.
mount /dev/sdc1 /media ----------This mount command is for the Backup Server or the 192.168.0.20 server.

Step 2
Assuming that you perform the step 1 correctly. Now go to your Ghost Script 2024 directory and type
cd /media/Ghost-Script.2024 -----For Backup Server if you mount your flash drive to Backup Server
cd /media/Ghost-Script.2024/mainServer--------For Main Server if you mount your flash drive to Main Server

Step 3
Since you finished step 2 very well. You are now in step 3 and you are now sending packages of file to its designated path or directory.
Now type this:
	./startConvert.sh then hit enter ---------- If you are performing for Backup Server
	./startCon.sh then hit enter ---------------- If you are performing for Main Server

You need to run this file in order to copy the package file to its designated directory that is configured by the author according to their function. After you run, you can now unmount your flash drive by typing this command:
				cd / then hit enter
				umount /media then hit enter			
Step 4
Next is type this at root terminal
cd /home/manager/main then hit enter
./sug.sh then hit enter and now it look like this below. Enter the password:ratbugasti then hit enter
 
Step 5
In System info Menu you can view the current information where the script is running. This info includes, motherboard, bios, disk drive, network, memory and POS type even the current serial. But the next step is you may select menu 4 or the SSH Key Generator.
 





Step 6
SSH Key Generator –The rule of this keygen is to bypass the current unix password. When you migrate the data from old server to new server they don’t need to require a password anymore during the script is running. After running SSH Key Generator you may now proceed to step 7.
 





Step 7
In this step, the only thing you do is just select menu 3 Run Conversion Script then hit enter. The script will start to copy the data that needed by the new server. Meanwhile the migration of data from old to new server are doing their job it may consume a several hours depending on the performance of the current old server. You can also monitored the progress of the number of files that being copy against the number of files that being copied. 
Note: In case you encounter a network traffic that may cause to hanging up of some terminals like TOS and POS terminal you can interrupt the process by just pressing Ctrl C or Ctrl Z and you can resume running menu 3 later when the hanging up is done or manageable. When it’s done you may now proceed to next step.
 


Step 8
Clear Cache After the migration of Data is done. You need to run menu number 2 or clear cache in order to clean some previous command or history command found on the server to avoid misused by the unaware user. Next you can now proceed to the next step.
 





Step 9
Exit Consider that you follow all the steps and the Data Migration is done successfully the next thing to do is to select Exit in order to wipe out all the file script packages that being sent to its designated path of the directory to the server to avoid misused.
Note: Selecting Menu 5 or Exit well wiped out all the file script to its designated path. In case you select it accidentally you may repeat the process or the step from the beginning.
 
All Rights Reserved 2024 Copyright by Ghost Script 2024 Created by: Mark Lester M. Lamanilao
