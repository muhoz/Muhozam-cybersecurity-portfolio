# Windows Server 2019 walkthrought

## 🎯The Objectives
In this project, I aim to:
- Install and configure Windows Server 2019 on Hyper-V.
- Set up and manage Active Directory and Group Policy.
- Configure and manage essential network services such as DHCP.
- Optimize the server's performance and security for enterprise deployment.
- Implement best practices for backup and disaster recovery.
- Monitor and troubleshoot server performance issues.

## The Skills Learned
Throughout this project, I acquired and enhanced the following skills:
- Utilizing Hyper-V for server virtualization.
- Proficiently installing and configuring Windows Server 2019.
- Deploying and managing Active Directory and Group Policy.
- Setting up and administering network service (DHCP) .
- Applying security best practices (password strategies).
- Developing backup and disaster recovery strategies.
- Monitoring server performance and troubleshooting common issues.

## 🛠️The Tools Used
The following tools and technologies were utilized in this project:
- **Windows Server 2019**: The primary operating system for the server.
- **Hyper-V**: For creating and managing virtual machines.
- **Active Directory**: For managing users, computers, and other resources.
- **Group Policy**: For centralized management and configuration of operating systems, applications, and users' settings.
- **DNS (Domain Name System)**: For translating domain names into IP addresses.
- **DHCP (Dynamic Host Configuration Protocol)**: For automating the assignment of IP addresses.
- **PowerShell**: For scripting and automation of server tasks.
- **Windows Admin Center**: For managing servers and clusters.
- **Microsoft Management Console**: To have all the tools we will be using during our work in the same place.



## Architecture of my HOMELAB
![Schéma de connexion des équipements](https://github.com/user-attachments/assets/a6e8c1da-2a1b-4eb3-8f4f-0bc1d5956aca)





## Steps

### Step 1: Installing Windows Server 2019 on Hyper-V
1. **Set up Hyper-V**: Ensure Hyper-V is installed and enabled on your host machine.
2. **Create a Virtual Machine**: Create a new virtual machine for Windows Server 2019.
3. **Install Windows Server 2019**: Mount the installation media and follow the setup wizard to install the OS.
4. **Initial Configuration**: Configure the server with an appropriate hostname, static IP address, and update settings.
5. **Setting up client hosts**: Installation and configuration of the two Windows 10 clients
6. **Setting up PFSense**: Installation and configuration of PFSense

 
### Step 2: Configuring Active Directory and Group Policy
1. **Install Active Directory Domain Services**: Use Server Manager to add the Active Directory Domain Services role.
2. **Promote to Domain Controller**: Configure the server as a new domain controller for a new forest.
3. **Create and Manage Users and Groups**: Use Active Directory Users and Computers to create organizational units, users, and groups.
5. **Configure Group Policy**: Create and link Group Policy Objects (GPOs) to enforce security and administrative settings.
6. **Configure MMC**: create and configure the MMC console so it can help us having all the controls at the same place

### Step 3: Managing Network Services (DHCP)
1. **Install and Configure DHCP**: Set up DHCP to automate IP address assignment.
2. **Create IP addresses range**: Define the range for the ip addresses for the clients
3. **Register the two client machines in the newly created forest**: Register the two clients with the users created

### Step 4: Performance Tuning and Security Best Practices
1. **Performance Monitoring**: Use Performance Monitor and Resource Monitor to track server performance.
2. **Optimize Performance**: Implement performance tuning techniques such as adjusting virtual memory, managing disk I/O, and network optimizations.
3. **Apply Security Best Practices**: Configure firewall rules, enable Windows Defender, and apply security updates.
4. **Audit and Monitoring**: Set up auditing policies and monitor logs for suspicious activities.

### Step 5: Backup and Disaster Recovery Planning
1. **Configure Windows Server Backup**: Set up regular backup schedules for critical data.
2. **Test Restore Procedures**: Ensure that backup data can be successfully restored.
3. **Develop a Disaster Recovery Plan**: Create a comprehensive disaster recovery plan outlining steps to recover from various failure scenarios.

### Step 6: Monitoring and Troubleshooting
1. **Set Up Monitoring Tools**: Use Windows Admin Center and other monitoring tools to keep track of server health.
2. **Identify and Resolve Issues**: Troubleshoot common server issues such as performance bottlenecks, service failures, and connectivity problems.
3. **Regular Maintenance**: Perform regular maintenance tasks such as checking for updates, reviewing logs, and cleaning up unnecessary files.



## ✨Keep an Eye Out for Updates!

This portfolio will expand as I earn more certifications and complete additional projects. I invite you to return to see my progress and discover more about my skills and experience.
Thank you for visiting. For further information, feel free to connect with me on my [LinkedIn](https://www.linkedin.com/in/yves-christian-muhozam) 
I will create folders for all the steps to detail the process every weeks.
