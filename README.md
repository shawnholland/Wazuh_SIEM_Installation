<h1>Wazuh SIEM Installation</h1>

 ### [Source Video](https://www.youtube.com/watch?v=QT81wcuoRFY&t=411s)
 ### [Source Guide](https://drive.google.com/file/d/1CDwjb5nSMaP73q2W-znWQpI6523oPxlI/view)

<h2>Description</h2>
Project consists of a simple PowerShell script that walks the user through "zeroing out" (wiping) any drives that are connected to the system. The utility allows you to select the target disk and choose the number of passes that are performed. The PowerShell script will configure a diskpart script file based on the user's selections and then launch Diskpart to perform the disk sanitization.
<br />


<h2>Tools and Applications Used</h2>

- <b>VirtualBox</b> 
- <b>Wazuh Manager/Agent</b>
- <b>CLI</b>

<h2>Environments Used </h2>

- <b>Windows 11</b>
- <b>Ubuntu</b>

<h2>Program walk-through:</h2>

<p align="center">
Create a Ubuntu virtual machine with VirtualBox: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/1.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Go into the settings of the newly created Ubuntu machine and change it's network adapter to "Bridged Network": <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/2.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Using a command to add a Wazuh GPG key: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/3.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/4.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Use commanmd to download and Execute Wazuh Installation: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/5.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Use the IP address of your Ubuntu machine and type it into the browser to access the Wazuh Dashboard: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/6.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
The username and password should have been given to you after the installation: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/7.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/8.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/9.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
On your windows machine download the Wazuh agent. Before downloading select version 4.12 (I tried the latest version and ran into conflicts): <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/10.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Download installer: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/11.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
In the Wazuh agent enter the IP of your Ubuntu device and press save: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/12.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Back on the Ubuntu machine, use command to add an Agent to our Wazuh: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/13.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Get the IP from the Windows device: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/14.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Use the windows IP for our new agent: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/15.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
We will get an authentication key after adding the agent and now it needs to be added to our windows device: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/16.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/17.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Restart the service: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/18.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Back on the Ubuntu machine go to the brower and refresh the page, you should now see our new agent we added: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/19.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/20.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Now that the connection between our devices is set up, this next part will be showing an example of how Wazuh can be a useful tool for file integrity monitoring. By adding a specific directory for wazuh to track in the ossec.conmf file, we can get real time updates of changes that are made to this directory remotely from our Ubuntu device: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/21.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Creating new directory for testing: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/22.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Restart the Wazuh agent: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/23.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Creating a fake file within the directory: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/24.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/25.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/26.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
I created a bunch more files just because it initially didn't show up in the events: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/27.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Now I can see real time updates on the Ubuntu machine: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/28.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Some information availible from one of the events: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/29.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Deleting fake files: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/30.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
Verifying I can see them being deleted on my Ubuntu machine: <br/>
<img src="https://github.com/shawnholland/Wazuh_SIEM_Installation/blob/main/docs/31.png?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
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
