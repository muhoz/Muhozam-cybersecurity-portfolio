# Windows Server 2019 walkthrought

## The Objectives
In this project, I aim to:
- Install and configure Windows Server 2019 on Hyper-V.
- Set up and manage Active Directory and Group Policy.
- Configure and manage essential network services such as DNS and DHCP.
- Optimize the server's performance and security for enterprise deployment.
- Implement best practices for backup and disaster recovery.
- Monitor and troubleshoot server performance issues.

## The Skills Learned
Throughout this project, I acquired and enhanced the following skills:
- Proficiently installing and configuring Windows Server 2019.
- Deploying and managing Active Directory and Group Policy.
- Setting up and administering network services including DNS and DHCP.
- Utilizing Hyper-V for server virtualization.
- Applying security best practices to safeguard server infrastructure.
- Developing backup and disaster recovery strategies.
- Monitoring server performance and troubleshooting common issues.

## The Tools Used
The following tools and technologies were utilized in this project:
- **Windows Server 2019**: The primary operating system for the server.
- **Hyper-V**: For creating and managing virtual machines.
- **Active Directory**: For managing users, computers, and other resources.
- **Group Policy**: For centralized management and configuration of operating systems, applications, and users' settings.
- **DNS (Domain Name System)**: For translating domain names into IP addresses.
- **DHCP (Dynamic Host Configuration Protocol)**: For automating the assignment of IP addresses.
- **PowerShell**: For scripting and automation of server tasks.
- **Windows Admin Center**: For managing servers and clusters.

## Architecture of my HOMELAB



## Steps

### Step 1: Installing Windows Server 2019 on Hyper-V
1. **Set up Hyper-V**: Ensure Hyper-V is installed and enabled on your host machine.
2. **Create a Virtual Machine**: Create a new virtual machine for Windows Server 2019.
3. **Install Windows Server 2019**: Mount the installation media and follow the setup wizard to install the OS.
4. **Initial Configuration**: Configure the server with an appropriate hostname, static IP address, and update settings.

### Step 2: Configuring Active Directory and Group Policy
1. **Install Active Directory Domain Services**: Use Server Manager to add the Active Directory Domain Services role.
2. **Promote to Domain Controller**: Configure the server as a new domain controller for a new forest.
3. **Create and Manage Users and Groups**: Use Active Directory Users and Computers to create organizational units, users, and groups.
4. **Configure Group Policy**: Create and link Group Policy Objects (GPOs) to enforce security and administrative settings.

### Step 3: Managing Network Services (DNS, DHCP)
1. **Install and Configure DNS**: Set up DNS to manage domain name resolution within your network.
2. **Create DNS Zones and Records**: Define forward and reverse lookup zones and create necessary DNS records.
3. **Install and Configure DHCP**: Set up DHCP to automate IP address assignment.
4. **Create and Manage Scopes**: Define DHCP scopes and options for different network segments.

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

