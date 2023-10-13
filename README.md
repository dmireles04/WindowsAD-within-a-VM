<h1>Windows AD within a Virtual Machine</h1>

<h2>Description</h2>

- Oracle VirtualBox was used to spin up 2 VMs.
  
- The first is configured to simulate an "employer" created Active Directory where 1000+ "employees" were populated into this AD

- The 2nd VM is used to simulate a newly created user (Bruce Wayne) actually using their credentials to access the the "employer's" server.
<br />


<h2>Utilities and Environments Used</h2>

<br />
<b>Oracle VirtualBox</b>
<img src="https://imgur.com/LgrfVh4.png" height="40%" width="40%" alt="Windows AD within a VM"/>
<br />
<b>Windows Server Manager</b>
<img src="https://imgur.com/bCJQ3ib.png" height="60%" width="60%" alt="Windows AD within a VM"/>
<br />
<b>Windows Active Directory</b>
<img src="https://imgur.com/5bK7cKU.png" height="60%" width="60%" alt="Windows AD within a VM"/>
<br />
<br />
<b>Windows 10</b> (21H2)
<br />
<br />
<br />
<h2>Program walk-through:</h2>

<p align="Left">
<b>Oracle VirtualBox Setup:<b> <br/>
<br /> 
- I have identified the separate virtual machines that I spun up for this specific project.  
<br />
- The VM highlighted by the yellow arrow is the one used to simulate an "employer" server and is where I created the Active Directory
<br />
- The VM highlighted by the green arrow is the one used to simulate the "employee" who was recently hired and will access the "employer's" server.
<img src="https://imgur.com/YOjXKRH.png" height="120%" width="120%" alt="Windows AD within a VM"/>
<br />
<br />
<br />
<br />
<b>"Employer" VM - Server Dashboard <b>  <br/>
<br />
- This is the "employer's" server dashboard and shows the various roles I created and showing as active
<img src="https://imgur.com/R6etKSX.png" height="120%" width="120%" alt="Windows AD within a VM"/>
<br />
<br />
<br />
<br />
<b>"Employer" VM - Server > Local Server Properties <b> <br/>
<br />
- This screenshot showcases the properties section of Local Server that was setup on the "employer" VM.
<br />
<img src="https://imgur.com/rmtu3eq.png" height="100%" width="100%" alt="Windows AD within a VM"/>
<br />
<br />
<br />
<br />
<b>Wazuh Dashboard -<b>
<b>Sample PCI DSS Rule-Related Event Log<b>  <br/>
<br />
 - This is an example of an event log that highlights the relevant Rule/Requirement Code ID # 
<br />
<img src="https://imgur.com/Bhs4pVa.png" height="100%" width="100%" alt="Windows AD within a VM"/>
<br />
<br />
<br />
<br />
<b>"Employer" VM - Active Directory<b>  <br/>
<br />
  - Here you can see the "employer's" Active Directory which is populated with over 10000 "current employees".  All the "employees" are simulated and do not represent any actual people.  
<br />
  - I've included a "new-hire" employee that we will refer to as Bruce Wayne, that is being added to the Active Directory.  I decided to promote Bruce to the "administrator" role, as shown further below.  
<img src="https://imgur.com/NZi5tvw.png" height="100%" width="100%" alt="Windows AD within a VM"/>
<br />
<br />
<br />
<br />
<b>"Employee" VM & "New Employee" Sign-In Screen<b>  <br/>
<br />
- Here, I showcase the "employer" VM highlighted in the yellow window on the left.  
<br />
Both VM were created with 4GB of Ram, and with approx 200 GB of SSD storage.
<br />
- The window to the right, highlighted by the green window, and simulates a new-hire "Bruce Wayne", currently looking at his "Screen-Lock" view.
<img src="https://imgur.com/qvSFlsG.png" height="100%" width="100%" alt="Windows AD within a VM"/>
<br />
<br />
<br />
<br />
<b>"Employee" - User access verfiied<b>  <br/>
<br />
-Bruce Wayne has verified his access is now active, and was able to confirm that he has "administrator" access now.
<img src="https://imgur.com/EbGmTXT.png" height="100%" width="100%" alt="Windows AD within a VM"/>
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
