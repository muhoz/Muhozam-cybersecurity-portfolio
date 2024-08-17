# Managing Network Services (DHCP)

## Installation and Configuration of the DHCP Server

DHCP : Dynamic Host Configuration Protocol is in simply words, a protocol that permits to assign the IP addresses of network devices dynamically.

### Installation of DHCP Server

In the Server Manager, to the top right corner, you will see the menus we will be using during our work. 
Click on the `Manage` > `Add Roles and Functionalities`.
Proceed as usual and Tick the `DHCP Services`, a window will appear, click on **Add functionalities** and **Next** until you reach the end and finally click on `Install`.
You can see in the left panel of the window, the list of your server with DHCP there.

<img width="579" alt="DHCP  installation finish" src="https://github.com/user-attachments/assets/92252e80-9db8-42b2-b071-f2b07be8cb86">


### Configuration

This one is easy, just click on the flag and `Next` till the end.


## Create IP addresses range
After the installation of the server is completed, we need to create a range of ip addresses where the server can pick to assign to the client (the device asking for an address).

Go to the top right corner of the Hyper-V Manager and open the `Tools`> `DHCP`.
This page show up :

<img width="488" alt="DHCP config page" src="https://github.com/user-attachments/assets/e0f6675d-f6bf-4bb0-9489-1d6d8cd0d7e6">



Right-click and choose the second option.
Fill the name and define the lower bound and upper bound of your ip addresses as follow (feel free to change the values).

<img width="490" alt="Screenshot 2024-08-11 123028" src="https://github.com/user-attachments/assets/f876ec3d-83f5-4b2b-b697-a4bda333e630">


<img width="385" alt="ip addresses range" src="https://github.com/user-attachments/assets/34c6ea5e-f56d-4db5-90bd-f8aac2d5a84a">


You can skip the next step until you are asked for the routeur address, fill in the address of your pfsense interface.



## Register the two client machines in the newly created forest

Turn on the first Windows 10 client and connect to the desktop and open the `system properties`

<img width="304" alt="Screenshot 2024-08-11 125357" src="https://github.com/user-attachments/assets/3d5849a2-df5a-4a5d-85b4-e071fa62b438">


Tick `Domain` and fill in with the name of your domain. You will be asked the account and password, input *misterx* or whatever name you created the user in the Domain controller.
Done, restart your computer and you will sign in with newly account.

<img width="771" alt="misterx" src="https://github.com/user-attachments/assets/eb40ed64-0f8c-4993-935c-92bcd24845fc">

Do the same for the second client (*missy*)

## Group Policy Object (GP0)

A group policy is "a virtual collection of policy settings, security permissions, and scope of management (SOM) that you can apply to users and computers", as defined by Microsoft on this link : https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/manage/group-policy/group-policy-overview.

In our example, we will create a gpo that helps to deploy a software on the computer in the domain.

Go to the top right corner of the Hyper-V Manager and open the `Tools`> `Group strategy`.
fffffff



Window opened, make a right cick as shown on the screeenshot and we will choose the first option :
fffffff

Create the group and assign it a name. Next, we will modify it:
ffffff

We have two options here:
Assign the GPO by users
Assign the GPO by computers

fffff

We will assign it by computers. This will permit the computer to have the GPO applied even if the user is changed after.
Follow these steps to create a new one



Now, choose the software you need to deploy (*it has to be a .msi package*). Wait until the software appears in the window :
It's seems to be good now, let's restart the windows clients to see if the strategy is applied.




