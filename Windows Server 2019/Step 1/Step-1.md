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
First thing is to get the ISO image for WS2019, which can be found at : <a href="https://go.microsoft.com/fwlink/p/?LinkID=2195167&clcid=0x409&culture=en-us&country=US">.
The evaluation expires after 180 days.

For the installaton process :
- on Hyper-V Manager, to your right, choose `New -> Virtual Machine...`
<img width="529" alt="Create_VM" src="https://github.com/user-attachments/assets/3e041eab-96fb-4142-9d7e-e15017293924">

- in the wizard, just follow the instructions and modify the settings for your VM as shown there  (insert the name, the location on your drive to store the VM files) :
<img width="530" alt="settings_of_DC" src="https://github.com/user-attachments/assets/57ef4cd2-03eb-4af2-b92e-9315b7cb0e9e">

