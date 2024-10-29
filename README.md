
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
Retrieve login attempts on specific dates:  <br/>
<br />
<img src="https://i.imgur.com/EjOYwgk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
In this case, use SELECT * FROM log_in_attempts. It will show all the columns in the login attempts table. Use WHERE login_date = ‘2022-05-09’ OR login_date = ‘2022-05-08’ ; that only specify those 2 dates which are the day issues occurred and 1 day before. OR means it will show all the information from those two dates. <br />
<br />
Retrieve login attempts exclude particular country: <br/>
<br />
<img src="https://i.imgur.com/HBwgIqD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
<br />
In this case, use SELECT * FROM log_in_attempts to query all columns on the login attempts table. Then, use WHERE NOT country = ‘Mexico’ ; to look search for login attempts that occur in all countries except Mexico. <br />
<br />
Retrieve employee list from particular department:  <br/>
<br /> 
<img src="https://i.imgur.com/F5RgaMK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
<br />
In this case, use SELECT * FROM employees to retrieve all columns (*) on the employee's table. Use WHERE department = ‘Marketing’ AND office = ‘East%’ ; to filter only Marketing employees in the East building that will be shown in queries. <br />
<br />
Retrieve employee list from multiple department:  <br/>
<br />
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
