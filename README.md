<h1>How to analyse a data packet (p-cap file) using wireshark</h1>



<h2>Description</h2>
In this Project i used Wireshark to inspect data packet file and applied filters to sort through packet information efficiently.
<br />


<h2>Utilities Used</h2>


- <b>Wireshark</b>

<h2>Environments Used </h2>

- <b>Virtual Box</b>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Launch wireshark on the network and capture: <br/>
<img src="https://i.imgur.com/Xdmyats.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

  - <b> A lot of network packet traffic is seen, which is why we’ll need to apply filters to find the information we need.

<br />


I applied a basic filter for traffic associated with a specific IP address which is 142.250.1.139:  <br/>
<img src="https://i.imgur.com/XmW8Mz9.png" height="80%" width="80%" alt="Data packet analysis"/>
<br />

<br />
This provides you with details about the overall network packet, or frame, including the frame length and the arrival time of the packet. here we see entire packet of data.: <br/>
<img src="https://i.imgur.com/qFhiYKI.png" height="80%" width="80%" alt="Data packet analysis"/>
<br />
<br />
At the Ethernet level, we see the source and destination MAC addresses and the type of internal protocol that the Ethernet packet contains:  <br/>
<img src="https://i.imgur.com/7T5xsdl.png" height="80%" width="80%" alt="Data packet analysis"/>
<br />
<br />
Now we want to see just the traffic from the specific destination IP address::  <br/>
<img src="https://i.imgur.com/O3oSYTX.png" height="80%" width="80%" alt="Data packet analysis"/>
<br />
<br />

We can also use filters to select and examine DNS traffic:  <br/>
<img src="https://i.imgur.com/QsgPIUM.png" height="80%" width="80%" alt="Data packet analysis"/>
<br />
<br />
You can also use additional filters to select and examine TCP packets as shown below:  <br/>
<img src="https://i.imgur.com/YItWWTt.png" height="80%" width="80%" alt="Data packet analysis"/>
</p>

There are definitely lots of filters that can be used to analyse this data packet file but just for the purposes of this project i chose to keep it simple and i hope it was helpful.

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
