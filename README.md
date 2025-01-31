# Create-and-Delete-User-with-Powershell-Cmdlet



<h2>Description</h2>
Project consists of a simple PowerShell commandlets to delete/create users and creating OUs. I also added how to move a user from one OU to another


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Active Directory Domain Contoller</b>

<h2>Environments Used </h2>

- <b>Windows 2019 server</b> (22H2)

<h2>Command script walk-through:</h2>

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
<br />
<br />
 Navigate to the Active Directory Users and Computers windows under tools on the top right Tab.: <br/>
<img src="https://i.imgur.com/wxdUBdR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
<br />
Find "Desktop Support", Right click on properties, navigate to "Object" and Deselect "Protect object from accidental deletion" box. Apply. Right click on "Desktop Support" and delete it:  <br/>
<img src="https://i.imgur.com/jmtyehK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br /> 
<br />
Go back to your PowerShell window and type in whats in the picture to create the OU again.:  <br/>
<img src="https://i.imgur.com/7N2sXSQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
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
In the users and computers window, click on View on the top and select Advanced features(this will be useful later):  <br/>
<img src="https://i.imgur.com/UXDe9gg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Find Jon Doe again under Users and right click and select Properties:  <br/>
<img src="https://i.imgur.com/ipqNoQS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select Attribute Editor (Advanced Features enables the option to view this tab):  <br/>
<img src="https://i.imgur.com/bz472Q6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Distinguished Name is used to move Jon Doe to the Desktop OU:  <br/>
<img src="https://i.imgur.com/AkTZtcz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go back to the Windows Powershell window and type in what in the picture. You can have the Attribute Editor window on the side to copy the Distinguished Name as well which goes after "-Identity":  <br/>
<img src="https://i.imgur.com/E5cpb2w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go back to the Users and Computers window and you should see Jon Doe under Desktop:  <br/>
<img src="https://i.imgur.com/GqL7PgH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
And Thats IT!!! (it but as IT as in info Tech)
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
