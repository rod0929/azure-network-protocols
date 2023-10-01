<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create Resources
- Install Wireshark
- Observe Differing Network Protocols

<h2>Actions and Observations</h2>

<p>The first step will be creating a Resource group that will house our two Virtual Machines to observe the traffic being sent between the two machines. To Create the Resource Group you can do a quick search for `Research Group ` at the top of Azure or you can select `Create a Resource` and then choose to create the Resource group from the Azure Market Place. 

<img src="https://i.imgur.com/GKUzeBu.png" height="70%" width="70%" alt="search resource group" /> 
</p>
<p>
After `Research Group` is entered and the results are returned, you can now select the `+ Create` button. This will begin the process of creating the resource group that will have eaach of our resources such as the virtual machines.  
<p align="center">
</p>
<br />

<p>
<img src="https://i.imgur.com/Tqk3vLR.png" height="80%" width="80%" alt="search and create resource group" />
</p>
<p>
You will select the `subscription name`, enter your custom created `resource group` (here enter RG-LAB-2) name and select the preferred `region` that is the nearest to you that would assist saving on cost. As you are creating the resource group, you will see the option to create  tags as well; however, in this lab, the tag is not needed.

</p>
<br />

<p>
<img src="https://i.imgur.com/Kwqp98O.png" height="60%" width="60%" alt="create resource group name" />
</p>
<p>
The two virtual machines that we create will allow us to send traffic between the two machines. You can name the Virtual Machine whatever you prefer to name them and can be easy to remember. 

</p>
<br />
