# Virtual-Machine-Enterprise-Enviroment-Set-up
## OverView
In this Lab I set up multiple virtual machines to build my own VM network with a Windows active directory enviroment with windows server and enterprise work stations. I am setting up this enviroment to use in future labs.

### Part 1: Initial Set Up and Deployment of the Windows Server**

**1)** Used Oracle VirtualBox to provision a VM and used a Windows Server ISO file  
![Server VM created](https://i.imgur.com/kO7O9mS.png)  

**2)** Before I launched the Server VM (**DC01**) I used the network tab in VirtualBox to set up a virtual Nat Network: **MyLabNet** and specified an IPv4 Prefix. I also disabled DHCP becuase I want I want Static IP addresses for my lab enviroment  
![NatNetwork](https://i.imgur.com/N7x7vfi.png)  

**3)** I went to the settings of **DC01** in VirtualBox and attached the network addapter to **MyNetLab**
![NEt Adaptor](https://i.imgur.com/DuIs87X_d.webp?maxwidth=760&fidelity=grand)  

**4)** Let the VM **DC01** download the ISO file and launch Windows Server  
![WinServ Launch](https://i.imgur.com/kKDrtFO.png)  

**5)** Used the command line in **DC01** to Set the IPv4 address, subnet mask, defualt gateway and DNS. 
![IP set up](https://i.imgur.com/wDJSDa0.png)  
![IP change](https://i.imgur.com/sDTPuIm.png)  

**6)** Used ipconfig to confirm Settings and pinged 1.1.1.1 to verify internet connection
![IPCONFIG](https://i.imgur.com/vvm1tVT.png)
