<h1>Drive Mapping by Group Policy</h1>

<h2>Description</h2>
A walkthrough of mapping a shared folder within a network by enforcing a group policy.
<br />


<h2>Prerequisites</h2>

- <b><a href="https://github.com/schul1012/Setting-up-network-of-a-domain-controller-and-a-client/tree/main">Setting up a Domain Controller and a Client, Using VirtualBox</a></b><br/>
- <b><a href="https://github.com/schul1012/Active-Directory-Domain-Setup/blob/main/README.md">Active Directory Domain Setup</a></b><br/>
- <b><a href="https://github.com/schul1012/NAT/tree/main">RAS and NAT configuration</b></a><br/>
- <b><a href="https://github.com/schul1012/DHCP/tree/main">DHCP</b></a><br/>


<h2>Environments Used</h2>

- <b>Windows 2019</b>

<h2>Walkthrough</h2>

<p align="center">
Click on 'Tools' - 'Group Policy Management' on Server Manager. <br/>
<img width="458" height="536" alt="image" src="https://github.com/user-attachments/assets/72a36d2b-eb69-4625-9446-2505827979cf" />
<br/>
<br/>

<p align="center">
Right-click on the domain, left-click on 'Create a GPO in this domain, and Link it here...', name the group policy and click 'OK'. Right-click on the new policy and click on 'Edit...'.<br/>
<img width="973" height="525" alt="image" src="https://github.com/user-attachments/assets/88b88003-623a-4542-9c37-b7cced786222" /><br/>

<br/>
<br/>

<p align="center">
Group Policy Management Editor will pop up. This time, I'll apply the policy rather to users than computers. Locate - 'User Configuration' - 'Preferences' - 'Windows Settings' - 'Drive Maps'. Right-click on the empty space on the right and then select 'New' - 'Mapped Drive'<br/>
<img width="1165" height="718" alt="image" src="https://github.com/user-attachments/assets/be90b326-3d83-4fad-92e3-b170e10cae00" />
<br/>
<br/>

<p align="center">
The location should be \\(server computer name)\(shared folder name). Click 'OK'.<br/>
<img width="395" height="451" alt="image" src="https://github.com/user-attachments/assets/ca9a3c30-a97b-47fb-9d26-b1ccff15bf0e" />
<br/>
<br/>
  
<p align="center">
I can now also set the target group, user or computers for this Group Policy on Group Policy Management.<br/>
<img width="964" height="514" alt="image" src="https://github.com/user-attachments/assets/98c47414-e00f-4b75-9621-a4aae59878e6" />
<br/>
<br/>

<p align="center">
The shared folder is now mapped on the client's File Explorer.<br/>
<img width="1017" height="841" alt="image" src="https://github.com/user-attachments/assets/82ba01e1-45c2-48f8-a548-496e071a17d7" />
<br/>
<br/>



