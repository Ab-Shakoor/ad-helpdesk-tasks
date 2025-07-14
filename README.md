<h1>Active Directory Help Desk Tasks</h1>


<h2>Overview</h2>
This section documents hands-on experience with common help desk responsibilities performed in my existing <a href="https://github.com/Ab-Shakoor/Active-Directory-Lab">Active Directory Home Lab</a>.
<br />

<h2>Objective</h2>
Gain hands-on experience and familiratiy with common every day Active Directory help desk tasks.

<h2>Tools Used</h2>

- <b>VirtualBox</b> 
- <b>Windows Server 2019</b>
- <b>Active Directory</b>

<h2>Key Features</h2>

- <b>Locate users and computers in AD</b> 
- <b>Reset user passwords</b>
- <b>Edit user attributes (title, department, phone)</b>
- <b>Move users between OUs</b>
- <b>Enable Advanced Features and view extra attributes</b>
- <b>View computer properties and trust status</b>
- <b>Create a service account with limited permissions</b>
- <b>Simulate onboarding (create new user and assign to group)</b>
- <b>Simulate offboarding (disable user and move to "Disabled Users" OU)</b>


<h2>Project walk-through:</h2>
<br/>

<p align="center">
<b>Used the "Find" tool in ADUC to locate a specific user by the name "abdullah":
<br/>
 
<br/>
<img src="https://i.imgur.com/DlKlKgh.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />
 
<br/>
<img src="https://imgur.com/RCQtWUN.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

 
<br/>

---

<p align="center"> 
<br />
Located user `ashakoor` in ADUC, right-clicked and selected “Reset Password”, and applied a temporary password and enforced a reset on next login: 
<br/>

<br/>
<img src="https://i.imgur.com/TFYrIi7.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Opened the properties for user `ashakoor` and updated job title and department: 
<br/>

<br/>
<img src="https://i.imgur.com/csFra62.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>
<img src="https://i.imgur.com/K3kTPgq.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>
<img src="https://i.imgur.com/jjYboJh.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Moved user `ashakoor` from `_USERS` to `IT_DEPARTMENT` OU:  
<br/>

<br/>
<img src="https://i.imgur.com/9Nc1i6a.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Enabled “Advanced Features” under the View menu and viewed `Attribute Editor` to inspect `lastLogon`:
<br/>

<br/>
<img src="https://i.imgur.com/zF0h0mJ.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Viewed the computer object for the Windows 10 client and confirmed domain membership and basic system info:  
<br/>

<br/>
<img src="https://i.imgur.com/lK7rpNk.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>
<img src="https://i.imgur.com/xpkDndF.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>
<img src="https://i.imgur.com/sDSDejP.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Created account `svc_backup` to act as service account, set password to never expire, unchecked login requirement, and added description to clarify purpose:  
<br/>

<br/>
<img src="https://i.imgur.com/4nreaxz.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>
<img src="https://i.imgur.com/S7tPFRV.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Created `ljackson` in `IT_DEPARTMENT` OU, Set password, and updated job title and department:</b>  
<br/>

<br/>
<img src="https://i.imgur.com/QD6POsD.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>
<img src="https://imgur.com/yCzZ1Wv.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Disabled `ljackson` and moved account to `Disabled Users` OU for archiving:</b>  
<br/>

<br/>
<img src="https://i.imgur.com/QD6POsD.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>
<img src="https://imgur.com/yCzZ1Wv.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
