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

You will have the window like this now
ffffff

And it's done, save your console to the desktop to reach it easily.
