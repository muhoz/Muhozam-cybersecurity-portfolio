<img width="771" alt="image" src="https://github.com/user-attachments/assets/0a15040c-eb59-4b48-94ff-6d0a0a03edf0"># Managing Network Services (DHCP)

## Installation and Configuration of the DHCP Server

DHCP : Dynamic Host Configuration Protocol is in simply words, a protocol that permits to assign the IP addresses of network devices dynamically.

### Installation of DHCP Server

In the Server Manager, to the top right corner, you will see the menus we will be using during our work. 
Click on the `Manage` > `Add Roles and Functionalities`.
Proceed as usual and Tick the `DHCP Services`, a window will appear, click on **Add functionalities** and **Next** until you reach the end and finally click on `Install`.
You can see in the left panel of the window, the list of your server with DHCP there.
fffffffffffffff

### Configuration

This one is easy, just click on the flag and `Next` till the end.

## Create IP addresses range
After the installation of the server is completed, we need to create a range of ip addresses where the server can pick to assign to the client (the device asking for an address).

Go to the top right corner of the Hyper-V Manager and open the `Tools`> `DHCP`.
This page show up :
fffffffffff

Right-click and choose the second option.
Fill the name and define the lower bound and upper bound of your ip addresses as follow (feel free to change the values).
fffffffff

You can skip the next step until you are asked for the routeur address, fill in the address of your pfsense interface.

## Register the two client machines in the newly created forest

Turn on the first Windows 10 client and connect to the desktop and open the `system properties`
ffffffffff

Tick `Domain` and fill in with the name of your domain. You will be asked the account and password, input *misterx* or whatever name you created the user in the Domain controller.
Done, restart your computer and you will sign in with newly account.
fffffffff


Do the same for the second client (*missy*)
