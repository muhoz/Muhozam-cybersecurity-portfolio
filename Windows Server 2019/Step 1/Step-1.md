# Setting-up Hyper-V in Windows 10/11
I was a client of VMWare and Virtual Box but after discovering Hyper-V and try it, i prefer to use this solution as an Hypervisor for my VMs.

So to install it (better say activate it), you can :
- On your search bar, you can enter "Features" and this will be shown
<img width="554" alt="features" src="https://github.com/user-attachments/assets/06e63bcc-66d9-444f-ac3a-61573237e7bf">


- After this window will shown, scroll till you find Hyper V and check all the box related
<img width="349" alt="turn_on_features" src="https://github.com/user-attachments/assets/7d1f5d6a-f3fe-4b2a-8644-e31f28c61344">


- Your computer will restart and you will be able to find "Hyper V Manager" by entering it on the search bar.
<img width="580" alt="hyperVManager" src="https://github.com/user-attachments/assets/50c39313-b298-4d25-8f8a-bd0661fd26c2">

- Click on it and the manager will show itself

# Create a VM (Windows Server 2019) 
First thing is to get the ISO image for WS2019, which can be found at : <a href="https://go.microsoft.com/fwlink/p/?LinkID=2195167&clcid=0x409&culture=en-us&country=US"> Windows Server 2019 </a>.
The evaluation expires after 180 days.

For the installaton process :
- On Hyper-V Manager, to your right, choose `New -> Virtual Machine...`
<img width="529" alt="Create_VM" src="https://github.com/user-attachments/assets/3e041eab-96fb-4142-9d7e-e15017293924">

- In the wizard, just follow the instructions and modify the settings for your VM as shown there  (insert the name, the location on your drive to store the VM files) :
<img width="530" alt="settings_of_DC" src="https://github.com/user-attachments/assets/57ef4cd2-03eb-4af2-b92e-9315b7cb0e9e">

The installation done, the VM will restart and ask you to enter the login (i used `Administrator`) and choose your password. Let Windows finish to start and all should be ok.

# Before continuing there is 2 things to do
## Configure the network interfaces we will be using in our work

For our work, we need 2 network interfaces as shown in the our network diagram :
- One connected to the WAN, which PFSense will be connected to. It will help us to gain connectivity from our WIFI card.
- One connected to the LAN, which will be the subnet including the two clients, the DC and the second interface of PFSense.

Let's start.
To create the two interfaces, we will go at the right of the Hyper-V Manager and open the `Virtual Switch Manager`
ffffffffff
In the window, create the two interfaces, one named External Switch as External type (connect it to the wifi card directly) and another Private Switch as a Private type.
Validate and close the window.

## The second thing, we will be setting up is the PFSense VM

PFSense is a free and open source firewall and router with a lot of benefits. We will make another projects specifically on it but for now, we will just use it as a router to route our LAN traffic to the Internet.
The VM is available at : [PFSENSE](https://www.pfsense.org/download/)

VM downloaded, we can install it like the Windows Server 2019. Just accept everything and pursue.
At this step, you have to setting up the two network interfaces:
- First one goes to the WAN that we created as the first one (hn0)
- Second one goes to the LAN (hn1)

And voilà, after the configuration ended, you will be facing this view : 
ffffff



Now that all our configurations are done, we can continue with the Windows Server 2019 configuration.
Start it and we will :
- Change the name of the computer to make it more memorable (something like SERVER2019). You will need to restart the computer after doing it.
- Computer restarted, we need to configure a static address for the network interface. Open the network configuration panel with a WIN+R and enter ncpa.cpl. The window opened, configure all the settings like in the screenshot:
ffffff
PS: please, if necessary, modify the addresses to meet your environment.

If the configuration is good, you will see the network icon as:
ffffffff




# Installation and Configuration of the two clients

As previously, we can download the ISO images on the Microsoft Evaluation Center and install it by following the same steps as the Windows Server 2019.
In the installation wizard, enter a username and password as desired.

After all this configuration, we will have the list of VMS as show here:
ffff
