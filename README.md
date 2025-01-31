# Create-and-Delete-User-with-Powershell-Cmdlet



<h2>Description</h2>
Project consists of a simple PowerShell commandlets to delete/create users and creating OUs. I also added how to move a user from one OU to another


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Active Directory Domain Contoller</b>

<h2>Environments Used </h2>

- <b>Windows 2019 serve</b> (22H2)

<h2>Command scipt walk-through:</h2>

<p align="center">
Launch "Windows PowerShell" as Administrator 
 *Do not run Windows PowerShell ISE: <br/>
<img src="https://i.imgur.com/JM4eoes.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Type in the code thats in the picture and type in "Y". We are using "Jdoe" since we have to use his sAMAccount name we created for him. We are removing Jon Doe to recreate him using powershell:  <br/>
<img src="https://i.imgur.com/jTFN0Ck.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to the Active Directory Users and Computers windows under tools on the top right Tab.: <br/>
<img src="https://i.imgur.com/wxdUBdR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Find "Desktop Support", Right click on properties, navigate to "Object" and Deselect "Protect object from accidental deletion" box. Apply. Right click on "Desktop Support" and delete it:  <br/>
<img src="https://i.imgur.com/jmtyehK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go back to your PowerShell window and type in whats in the picture to create the OU again.:  <br/>
<img src="https://i.imgur.com/7N2sXSQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Type what is in the picture to create Jon Doe again:  <br/>
<img src="https://i.imgur.com/LbhnZKu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to users and computers again form your taskbar. If you closed the window, you can go to tools and open it again:  <br/>
<img src="https://i.imgur.com/wxdUBdR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 Navigate to "Users" and Jon Doe should be on the bottom. If you can't find the name, you can search for him with the search tool on the top with the magnifying glass:  <br/>
<img src="https://i.imgur.com/0OR0o0R.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Type Jon Doe in the search bar and click on "Find Now" and he should pop up:  <br/>
<img src="https://i.imgur.com/fxHYMf7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
