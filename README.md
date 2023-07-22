<p align="center">
<img src="https://i.imgur.com/QurLqjG.png" height="40%" width="60%"/>
</p>

<h1>Observing the Effect of a VPN on IP Addressing</h1>
In this project, I conducted observations to understand how a virtual private network (VPN) affects IP addresses, locations, and web browsing activities. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
-	Remote Desktop
-	ProtonVPN (free version)


<h2>Operating System Used </h2>

- Windows 10 (21H2)

<h2>High-Level Steps</h2>

-	Create a Windows 10 virtual machine in Azure
-	Remote Desktop into the virtual machine
-	Use whatismyipaddress.com to find the IP address and location for the VM
-	Download the free version of ProtonVPN (create an account if there is no preexisting account)
-	In ProtonVPN, connect to a server in another country
-	Use whatismyipaddress.com to find the new IP address and location for the VM
-	Browse a webpage to see if there are any changes to the URL or language
-	Delete Resource Groups in Azure


<h2>Synopsis</h2>

![image](https://github.com/jtowns14/vpn-usage/assets/139197948/d0ad13c0-5ecc-43dc-aae8-556e5b9a1c20)

<p>


</p>
<p>
In this lab, the initial step involved setting up a Windows 10 VM in Azure, specifically choosing South Africa North as the VM's location within the "Essentials" section. After obtaining the public IP address, I connected to the VM using Remote Desktop.
</p>
<br />

![image](https://github.com/jtowns14/vpn-usage/assets/139197948/57f852a2-e5d8-4c31-bfee-6ab9cfd7d537)


<p>

</p>
<p>
After accessing the VM, I used Microsoft Edge to search for "whatismyipaddress.com," which displays the IP address and location. Since the website is accessed within the VM, it shows the same IP address assigned by Microsoft Azure (located in the top left corner). Additionally, the VM's Region was set to South Africa North (distinct from my actual location), and the website indicated the IP location as Johannesburg, South Africa.
</p>
<br />

![image](https://github.com/jtowns14/vpn-usage/assets/139197948/c4ade3cb-6a50-4c8b-b015-54055258471c)


<p>

</p>
<p>
Having acquired information about the VM's IP address and location, let's explore how it alters when utilizing a VPN. To conduct this experiment, I had already set up a free ProtonVPN account and proceeded to log in, followed by downloading the ProtonVPN software.
</p>
<br />

![image](https://github.com/jtowns14/vpn-usage/assets/139197948/0ef49c68-03e3-40f4-ad10-c0a4f624b3fa)


<p>

</p>
<p>
After choosing a server in Japan, I observed the alterations in ProtonVPN. Notably, one significant change was that my VPN's IP address differed from the VM's IP address (comparing the IP addresses in the top left corner of my screen and the VPN).
</p>
<br />

![image](https://github.com/jtowns14/vpn-usage/assets/139197948/e944c741-11c1-4fd1-b653-e3d5fca516cb)


<p>

</p>
<p>
Since I had whatismyipaddress.com already open in the Edge browser, I refreshed the page to observe any modifications. According to the website, my IP address now matched the one displayed in the VPN, and my location appeared as Tokyo, Japan. This occurred due to my physical computer being connected to the VM, which, in turn, was linked to a VPN server in Japan, creating the impression to the website that I was located in Japan.
</p>
<br />

![image](https://github.com/jtowns14/vpn-usage/assets/139197948/b9a04fc3-61eb-4dc1-a10f-cb7660b1cb62)


<p>

</p>
<p>
By looking up "neftlix" using Google, the search results appeared in Japanese, solidifying the VPN's successful implementation.
</p>
<br />

<p>
✨ And that’s what happens when you use a VPN!
</p>
<br />
