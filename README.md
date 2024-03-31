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
<br />
description  <br/>
<img src="https://i.imgur.com/FTDyEQW.png" height="80%" width="80%" alt="2"/>
<img src="https://i.imgur.com/P5wvhvA.png" height="80%" width="80%" alt="3"/>
<img src="https://i.imgur.com/mwQw4nM.png" height="80%" width="80%" alt="4"/>
<img src="https://i.imgur.com/zajx2zd.png" height="80%" width="80%" alt="5"/>
<img src="https://i.imgur.com/Ko9DKgk.png" height="80%" width="80%" alt="6"/>
<img src="https://i.imgur.com/kItqBI5.png" height="80%" width="80%" alt="7"/>
<img src="https://i.imgur.com/fSrrxUw.png" height="80%" width="80%" alt="8"/>
<img src="https://i.imgur.com/4Vw4cVS.png" height="80%" width="80%" alt="9"/>
<img src="https://i.imgur.com/u36Xcun.png" height="80%" width="80%" alt="10"/>
<img src="https://i.imgur.com/pHZJLPz.png" height="80%" width="80%" alt="11"/>
<img src="https://i.imgur.com/3w6VRbs.png" height="80%" width="80%" alt="12"/>
<img src="https://i.imgur.com/dyCk0mt.png" height="80%" width="80%" alt="13"/>
<img src="https://i.imgur.com/y1Fyylj.png" height="80%" width="80%" alt="14"/>
<img src="https://i.imgur.com/JGyiKa2.png" height="80%" width="80%" alt="15"/>
<img src="https://i.imgur.com/h9irt70.png" height="80%" width="80%" alt="16"/>
<img src="https://i.imgur.com/srZdzS9.png" height="80%" width="80%" alt="17"/>
<img src="https://i.imgur.com/KEu48DE.png" height="80%" width="80%" alt="18"/>
<img src="https://i.imgur.com/knbnUZS.png" height="80%" width="80%" alt="19"/>
<img src="https://i.imgur.com/cGcdQaL.png" height="80%" width="80%" alt="20"/>
<img src="" height="80%" width="80%" alt="21"/>
<img src="" height="80%" width="80%" alt="22"/>
<img src="" height="80%" width="80%" alt="23"/>
<img src="" height="80%" width="80%" alt="24"/>
<img src="" height="80%" width="80%" alt="25"/>
<img src="" height="80%" width="80%" alt="26"/>
<img src="" height="80%" width="80%" alt="27"/>
<img src="" height="80%" width="80%" alt="28"/>
<img src="" height="80%" width="80%" alt="29"/>
<img src="" height="80%" width="80%" alt="30"/>
<img src="" height="80%" width="80%" alt="31"/>
<img src="" height="80%" width="80%" alt="32"/>
<img src="" height="80%" width="80%" alt="33"/>
<img src="" height="80%" width="80%" alt="34"/>
<img src="" height="80%" width="80%" alt="35"/>
<img src="" height="80%" width="80%" alt="36"/>
<img src="" height="80%" width="80%" alt="37"/>
<img src="" height="80%" width="80%" alt="38"/>
<img src="" height="80%" width="80%" alt="39"/>
<img src="" height="80%" width="80%" alt="40"/>
<img src="" height="80%" width="80%" alt="41"/>
<img src="" height="80%" width="80%" alt="42"/>
<img src="" height="80%" width="80%" alt="43"/>
<img src="" height="80%" width="80%" alt="44"/>
<img src="" height="80%" width="80%" alt="45"/>
<img src="" height="80%" width="80%" alt="46"/>
<img src="" height="80%" width="80%" alt="47"/>
<img src="" height="80%" width="80%" alt="48"/>
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
