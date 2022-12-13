# Introduction

Veeam Backup & Replication comes with the PowerShell extension, a Veeam Backup PowerShell module that is added to your machine when you either install Veeam Backup & Replication server or the Veeam Backup & Replication Console. 

The Veeam Backup PowerShell module allows you to do almost all operations that are available in the user interface. Keep in mind that actions performed with PowerShell have the same force as actions performed using Veeam Backup & Replication.

Each cmdlet acts as a single-function command that can perform multiple operations with these objects. Objects represent instances of the Veeam backup infrastructure: jobs, databases, restore sessions and so on.

# Requirements

- A machine that runs the PowerShell session must have Windows PowerShell version 5.1 or later installed.
- The native console installed in Veeam Backup & Replication UI.

# Sessions

## Running Veeam PowerShell session from Veeam Backup Server

You can start a Veeam PowerShell session either using the Veeam Backup & Replication UI, or directly from the Windows PowerShell console installed on your machine.

- Using the Veeam Backup & Replication UI: in the main menu of Veeam Backup & Replication, select Console > PowerShell.
- From Windows PowerShell console: start the console on your machine.

![starting_from_vbr](https://user-images.githubusercontent.com/115532735/207282818-742da94c-3ff5-4016-97a7-7c6e7fd1d2ed.png)

## Running Veeam PowerShell Session from Remote Machine

The remote machine from which you run Veeam PowerShell commands must have the Veeam Backup & Replication Console installed. After you install the Veeam Backup & Replication Console, Veeam PowerShell module will be installed by default. 

Follow this [link](https://helpcenter.veeam.com/docs/backup/vsphere/install_console.html?ver=110) to get more information. 

# Scripts

The script named "Veeam_B&R_Configuration.ps1" performs the following tasks:

- Management of credentials
- Management of backup repositories
- Management of Veeam agents (credentials and containers)
- Management of protection groups
- Jobs management

This script is general purpose, it is made to configure Veeam globally.

### Sources 
[Veeam Documentation](https://helpcenter.veeam.com/docs/backup/powershell/getting_started.html?ver=110)
