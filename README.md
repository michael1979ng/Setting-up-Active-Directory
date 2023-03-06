# Setting-up-Active-Directory

This guide will cover the following.

Create an Isolated network using 192.168.20.0/24 network. The Active Directory test network will not have access to other networks or have internet. You can change this but is not recommended.
Create two virtual machines (Windows Server 2019, Windows 10 Enterprise).
You will create a new Active Directory forest using mylab.local for the domain.
Bulk create 21 organizational units using PowerShell.
Bulk create 20 security groups using PowerShell
Bulk import 3,000 user accounts using PowerShell.

Hardware Requirments:

Most computers and laptops should have no problem running multiple virtual machines. Below are the minimum requirements:

Any intel or AMD processor will do. Windows Server 2019 requirement is 1.4 GHz 64-bit processor.
6GB to 8GB RAM
50 GB free disk space
I’m using a Dell XPS 13 laptop and I have no issues running multiple virtual machines.

PowerShell Scripts:

Download the scripts below and place them in the c:\it folder on the Active Directory server.

Download Scripts Here

Included scripts:

create_groups.ps1 = Script for bulk creating AD security groups from the groups.csv file
create_ous.ps1 = This script will create the organizational units using the ous.csv file.
create_users.ps1 = This script will bulk import 3,000 users and place them in organizational units.
