# Installation and configuration of Active directory

## What is Active directory?

As defined by Microsoft, "A directory is a hierarchical structure that stores information about objects on the network. A directory service, such as Active Directory Domain Services (AD DS), provides the methods for storing directory data and making this data available to network users and administrators".

I don't want to take more time to talk about the AD DS concepts because there are a lot of ressources on the internet where you can get all the informations you neeed. I just leave this link from the Microsoft website, which i think explained very well all of the concepts:
https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview

## Installation of AD DS

In the Server Manager, to the top right corner, you will see the menus we will be using during our work. Click on the `manage` > `Add Roles and functionalities`.
Click on Next until you reach this page
ffffffffff

tick the `AD DS Services`, a window will appear, click on Add functionalities and Next until you reach the end and finally click on `Install`.
Process done, we will need to promote our server to be the DC controller. For this, follow these steps
Click on promote the server
fffffff

Tick the new forest and add a name in the XXXX.YYYY format:
ffffffff

Add a password for the DSRM :
fffffff

NetBios will fill the name automatically, just wait :
fffffff

Click Next, Install and wait for the installation to finish. 
ffffff

## Create and Manage Users and Groups
In this part, we will create two users: Mister X and Miss Y.
Mister X is working in the IT department as a technician and Miss Y is an accountant in our scenario.

### Creation of the two OUs (IT and COMPATBILITY)

Go to the top right corner of the Hyper-V Manager and open the AD users and computers
ffffff

This window will appear, do a right click on the DC name > New > Organisational Unit.
The OUs are represented as sub-folders within the DC main folder.

### Creation of the two users

Right click on the subfolder name for the concerned user > New > User.
Fill in the asked info and add a password in the next window.
fffff
fffff

Do as the same for Mister X

## Configure Group Policy


## Configure MMC
The Microsoft Management Console helps us to have a central management place where we can easily and rapidly reach the different functionalities we need.
To open it, execute the `MMC.exe` and follow the steps ( follow the red squares) :
ffffff


<img width="597" alt="Screenshot 2024-07-28 175401" src="https://github.com/user-attachments/assets/ce6e9225-5068-487c-b1f5-3e6074a9ff4b">
<img width="504" alt="Screenshot 2024-07-28 175017" src="https://github.com/user-attachments/assets/a66fbb73-b823-45b9-9c7b-2982ccfaed2d">
<img width="440" alt="Screenshot 2024-07-28 174732" src="https://github.com/user-attachments/assets/cd60bd1d-a966-481f-baaf-05a0888b9f55">
<img width="325" alt="Screenshot 2024-07-28 174018" src="https://github.com/user-attachments/assets/9770641f-ee4b-46e7-a9c5-61e2d068696e">
<img width="328" alt="Screenshot 2024-07-28 173857" src="https://github.com/user-attachments/assets/0191e54f-2a2e-42fe-afd5-54e8ddfaf2c0">
<img width="566" alt="Screenshot 2024-07-28 173442" src="https://github.com/user-attachments/assets/57a3efa3-f916-434c-85ef-05c0d7b40dd8">
<img width="599" alt="Screenshot 2024-07-28 171554" src="https://github.com/user-attachments/assets/f5704c55-5049-4b7b-9e75-a11fdcd1e0b5">
<img width="602" alt="Screenshot 2024-07-28 171412" src="https://github.com/user-attachments/assets/1767852d-579b-4a4d-bac0-d67ad59b00ac">
<img width="602" alt="Screenshot 2024-07-28 171126" src="https://github.com/user-attachments/assets/31a5cd86-3227-4544-a9cc-08da7dca7a2c">
<img width="589" alt="Screenshot 2024-07-28 170712" src="https://github.com/user-attachments/assets/cc46eb1d-8e4b-4544-9df9-1767476dca0e">
<img width="599" alt="Screenshot 2024-07-28 172625" src="https://github.com/user-attachments/assets/57a310a0-7a81-4efc-ab60-61dca475d83a">

You will have the window like this now
ffffff

And it's done, save your console to the desktop to reach it easily.
