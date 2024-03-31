<h1>Active Directory Home Lab</h1>

<h2>Description</h2>
In this lab I'm going to demonstrate how I created a home lab and configured Active directory on a domain controller using vmware. While configuring and running the lab environment I will configure Windows server 2019 to run the following services; DHCP, DNS, Splunk, NAT. 
I run attacks on a machine and used splunk to analyze the logs.
<br />


<h2>Tools Used</h2>

- <b>Active Directory</b>
- <b>Wireshark</b>
- <b>Splunk</b>
- <b>Vmware</b>
- <b>Vmware</b>

<h2>Environments Used </h2>

- <b>Windows Server 2019</b> 
- <b>Windows 10</b> 
- <b>Kali Linux</b> 

<h2>Walk-through:</h2>

<p align="center">
Network diagram: <br/>
<img src="https://i.imgur.com/T8PExrw.jpeg" height="60%" width="60%" alt="1"/>
<br />
Then I downloaded and installed VMware with a Windows 10 os for the target system, a Kali Linux os for the attacker and 2 Windows Server 2019 operating systems for the Active Directory server and Splunk server. Downloaded splunk and installed it into one of the Windows 2019 server vm.<br />
<br />
I assigned the ip addresses of each device to reflect my diagram.   <br/>
<img src="https://i.imgur.com/FTDyEQW.png" height="80%" width="80%" alt="2"/>
<img src="https://i.imgur.com/P5wvhvA.png" height="80%" width="80%" alt="3"/>
<br />
I checked connectivity between the servers on the network using ping, it timed out so I turned off the firewall and ping again and it’s connected. <br />
<img src="https://i.imgur.com/mwQw4nM.png" height="80%" width="80%" alt="4"/>
<br />I added a second network adapter to the server that will be the domain controller for internet connectivity. <br />
<img src="https://i.imgur.com/zajx2zd.png" height="80%" width="80%" alt="5"/>
<br />
I then added a role to server manager and installed active directory domain services to windows server 2019.  <br />
<img src="https://i.imgur.com/Ko9DKgk.png" height="80%" width="80%" alt="6"/> 
<img src="https://i.imgur.com/kItqBI5.png" height="80%" width="80%" alt="7"/>
 <br />
Then I configured the domain and restarted the server. <br />
<img src="https://i.imgur.com/fSrrxUw.png" height="80%" width="80%" alt="8"/>
<img src="https://i.imgur.com/4Vw4cVS.png" height="80%" width="80%" alt="9"/>
<br />
 I then created an organizational unit named “admins” for my administrator account. <br />
<img src="https://i.imgur.com/u36Xcun.png" height="80%" width="80%" alt="10"/>
<img src="https://i.imgur.com/pHZJLPz.png" height="80%" width="80%" alt="11"/>
<br />
 Then I added a user to create my account. <br />
<img src="https://i.imgur.com/3w6VRbs.png" height="80%" width="80%" alt="12"/>
<img src="https://i.imgur.com/dyCk0mt.png" height="80%" width="80%" alt="13"/>
<br />
 After creating the account I added it to the group of Domain Admins. <br />
<img src="https://i.imgur.com/y1Fyylj.png" height="80%" width="80%" alt="14"/>
<br />
 Then I add another role to the server for NAT. <br />
<img src="https://i.imgur.com/JGyiKa2.png" height="80%" width="80%" alt="15"/>
<img src="https://i.imgur.com/h9irt70.png" height="80%" width="80%" alt="16"/>
<img src="https://i.imgur.com/srZdzS9.png" height="80%" width="80%" alt="17"/>
<br />
 Then I configured the NAT and choose the NIC with DHCP. <br />
<img src="https://i.imgur.com/KEu48DE.png" height="80%" width="80%" alt="18"/>
<img src="https://i.imgur.com/knbnUZS.png" height="80%" width="80%" alt="19"/>
<img src="https://i.imgur.com/cGcdQaL.png" height="80%" width="80%" alt="20"/>
<br />
 Next I added a DHCP server to assign IP addresses to other computers in the network. <br />
<img src="https://i.imgur.com/YOt8ikI.png" height="80%" width="80%" alt="21"/>
<br />
 Then I configured the DHCP scope to assign IP addresses from a range of 192.168.11.12-100. <br />
<img src="https://i.imgur.com/YHFV7fM.png" height="80%" width="80%" alt="22"/>
<img src="https://i.imgur.com/fR4h7nJ.png" height="80%" width="80%" alt="23"/>
<img src="https://i.imgur.com/P978F8f.png" height="80%" width="80%" alt="24"/>
<img src="https://i.imgur.com/1yqIyPL.png" height="80%" width="80%" alt="25"/>
<img src="https://i.imgur.com/Z03ijJj.png" height="80%" width="80%" alt="26"/>
<img src="https://i.imgur.com/ug8Wmos.png" height="80%" width="80%" alt="27"/>
<img src="https://i.imgur.com/o7CbYum.png" height="80%" width="80%" alt="28"/>
<br />
 
<img src="https://i.imgur.com/xqjlQEV.png" height="80%" width="80%" alt="29"/>
<img src="https://i.imgur.com/4XBrJUs.png" height="80%" width="80%" alt="30"/>

<img src="https://i.imgur.com/pPgal9f.png" height="80%" width="80%" alt="31"/>

<img src="https://i.imgur.com/rP8Oo4H.png" height="80%" width="80%" alt="32"/>

<img src="https://i.imgur.com/UfUTE4j.png" height="80%" width="80%" alt="33"/>

<img src="https://i.imgur.com/f0iNHCk.png" height="80%" width="80%" alt="34"/>

<img src="https://i.imgur.com/54S3jZ7.png" height="80%" width="80%" alt="35"/>

<img src="https://i.imgur.com/7Ti2OPJ.png" height="80%" width="80%" alt="36"/>

<img src="https://i.imgur.com/xGEWoIC.png" height="80%" width="80%" alt="37"/>

<img src="https://i.imgur.com/eQ7M3ep.png" height="80%" width="80%" alt="38"/>

<img src="https://i.imgur.com/2sfeEIr.png" height="80%" width="80%" alt="39"/>

<img src="https://i.imgur.com/6OfLPt5.png" height="80%" width="80%" alt="40"/>

<img src="https://i.imgur.com/R2oPtmY.png" height="80%" width="80%" alt="41"/>

<img src="https://i.imgur.com/tbJyhyr.png" height="80%" width="80%" alt="42"/>

<img src="https://i.imgur.com/ipTJB7U.png" height="80%" width="80%" alt="43"/>

<img src="https://i.imgur.com/RuUO7fm.png" height="80%" width="80%" alt="44"/>

<img src="https://i.imgur.com/2MSQ75o.png" height="80%" width="80%" alt="45"/>

<img src="https://i.imgur.com/qoLP2Wk.png" height="80%" width="80%" alt="46"/>

<img src="https://i.imgur.com/BkLZ4N5.png" height="80%" width="80%" alt="47"/>

<img src="https://i.imgur.com/DkFQBw8.png" height="80%" width="80%" alt="48"/>

<img src="" height="80%" width="80%" alt="49"/>
<img src="" height="80%" width="80%" alt="50"/>
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
