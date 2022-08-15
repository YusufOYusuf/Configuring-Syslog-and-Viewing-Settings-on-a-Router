<h1>Configuring Syslog and Viewing Settings on a Router</h1>


<h2>Description</h2>
In this lab, I learned to configure Syslog and view settings on a router. Syslog is a logging solution that consists of two primary components: Syslog servers (which receive and store log messages sent from Syslog clients) and Syslog clients (which can be a variety of network devices that send logging information to a Syslog server).
<br />



<h2>Environments Used </h2>

- <b>Ubuntu 20.04.2 LTS</b> 
- <b>PuTTY SSH Client</b>

<h2>Program walk-through:</h2>

<p align="center">
From the left sidebar click PuTTY SSH Client and proceed to put in the IP address, port number, click Telnet and then click open: <br/>
<img src="https://i.postimg.cc/3rmrB9Gg/Screen-Shot-2022-08-14-at-6-17-20-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
In the R4 terminal window type the following commands <br/>
1. configure terminal <br/>
2. logging console 7 <br/>
3. logging monitor debug <br/>
4. logging buffered 4 <br/>
5. logging host 192.168.2.100 <br/>
6. logging trap warning <br/>
7. end <br/>
<img src="https://i.postimg.cc/CKjCVX6w/Screen-Shot-2022-08-14-at-6-22-03-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
In the R4 terminal window type "show logging" command to display the configured log settings<br/>
You can also hit your keyboard space bar to view more <br/>
<img src="https://i.postimg.cc/GmMP3vb5/Screen-Shot-2022-08-14-at-6-24-25-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
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
