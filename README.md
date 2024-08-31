<h1>Managing authorization </h1>



<h2>Description</h2>
In this lab, I used Linux commands in the Bash shell to learn how to examine and manage file permissions as well as configure user authorzation. 
<br />


<h2>Practical experience gained in this Lab</h2>

- <b>examine file and directory permissions</b> 
- <b>change permissions on files</b>
- <b>change permissions on directories</b> 


<h2>Environments Used </h2>

- <b>Qwiklabs</b> 

<h2>Lab walk-through:</h2>

<h2>Task 1: Check file and directory details file </h2>
In this task, I explored the permissions of the projects directory and the files it contains.
<p align="center"> <br/>
(1) I used the command "cd projects" to navigate to the projects directory. <br/>
(2) I used the command "ls -l" to list the contents and permissions of the projects directory. <br/>
(3) I used the command "ls -la" to check whether any hidden files exist in the projects directory and found that .project_x.txt is a file hidden in the projects directory.  <br/>
<img src="https://imgur.com/W9MmClD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br />
<br />
<h2>Task 2: Change file permissions </h2>
In this task, I need to determine whether any files have incorrect permissions and then change the permissions as needed. This action will remove unauthorized access and strengthen security on the system. <br/>
<p align="center">  <br/>
(4) I used the command "ls -l" to check whether any files in the projects directory have write permissions for the owner type of other. <br/>
(5) I used the command "chmod o-w project_k.txt" to change the permissions of the file identified in the previous step so that the owner type of other doesn't have write permissions. <br/>
(6) I used the command "chmod g-r project_m.txt" to change permissions of the project_m.txt file so that the group doesn't have read or write permissions. 
<img src="https://imgur.com/DZSGz7N.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br />
<br />
<h2>Task 3: Change file permissions on a hidden file </h2>
In this task, I need to determine if a hidden file has incorrect permissions and then change the permissions as needed. This action will further remove unauthorized access and strengthen security on the system.
<p align="center"> <br/>
(7) I used the command "ls -la" to check the permissions of the hidden file .project_x.txt. <br/>
(8) I used the command "chmod u-w,g-w,g+r .project_x.txt" to change the permissions of the file .project_x.txt so that both the user and the group can read, but not write to, the file.  <br/>
<img src="https://imgur.com/mxt8YgW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br />
<br />
<h2>Task 4: Change directory permissions file </h2>
In this task, I need to change the permissions of a directory. Only the 'researcher2' user should be allowed to access the `drafts` directory and its contents. (This means that only `researcher2` should have execute privileges.)
<p align="center"> <br/>
(9) I used the command "ls -la to check the permissions of the 'drafts' directory. <br/>
(10) I used the command "chmod g-x drafts" to remove the execute permission for the group from the drafts directory. <br/>
<img src="https://imgur.com/Il1XhsC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br />
<br />
