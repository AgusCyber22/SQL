
<h1> SQL - Security Operation</h1>


<h2>Description</h2>
Project consists of applying filter on SQL quaries to find malicious activity that might be potential security issues for company. 

<h2>Languages and Utilities Used</h2>

- <b>SQL</b> 

<h2>Environments Used </h2>

- <b>Linux</b> (VM)

<h2>Project walk-through:</h2>

<p align="center">
Retrieve after-hours failed login attempts: <br/>
<br /> 
<img src="https://i.imgur.com/tUpqVEY.png" height="80%" width="80%" alt="Retrieve after-hours failed login attempts"/>
<br /> 
<br />
Use SELECT * FROM log_in_attempts for query data in every column on the login attempts table. Then, use WHERE login_time > ‘18:00’ for search login attempts that happen after 18.00 which is hours after working office time. Success = 0 which means failed login.
<br />
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
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
