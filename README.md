<h1>Active Directory Home Lab</h1>


<h2>Overview</h2>
This section documents hands-on experience with common help desk responsibilities performed in my existing Active Directory home lab.

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


<h2>Network Diagram:</h2>
<br/>

<p align="center">
<img src="https://imgur.com/zmWOdUd.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>


<h2>Project walk-through:</h2>
<br/>

<p align="center">
<b>Configured Windows Server 2019 VM with two network interfaces: one for external internet access (NAT), one for internal domain traffic:
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
Assigned a static IP to the internal NIC so the domain controller can act as a DNS and DHCP server on the internal network: 
<br/>

<br/>
<img src="https://i.imgur.com/TFYrIi7.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Installed Active Directory Domain Services and promoted the server to a domain controller by creating a new forest and root domain. Logged in as the domain administrator after reboot: 
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
Created an Organizational Unit (OU) for administrative accounts and added a new domain admin user with elevated privileges:  
<br/>

<br/>
<img src="https://i.imgur.com/9Nc1i6a.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Enabled NAT on the domain controller using Routing and Remote Access, allowing internal network clients to access the internet:
<br/>

<br/>
<img src="https://i.imgur.com/zF0h0mJ.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Installed DHCP Server role and created a scope to assign IP addresses automatically to internal network clients:  
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
Used a PowerShell script to automate the creation of 1000 user accounts for testing purposes:  
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
Created a Windows 10 VM, connected it to the internal network, and successfully joined it to the domain:</b>  
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
