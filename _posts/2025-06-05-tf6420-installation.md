---
layout: post
title: TF6420 - TwinCAT 3 Database Server | Installation
date: 2025-06-05 15:24 -0300
categories: [TF6420 - TwinCAT 3 Database Server]
tags: [TwinCAT 3, TF6420, TwinCAT 3 Database Server]
---
> Remember that this page isn't affiliated with BECKHOFF and **MUST NOT** be used as official documentation. For that, please refer to the official BECKHOFF webpage.  
{: .prompt-danger }

> All content is free, and the main goal is to provide TUTORIALS. If you plan to use ANY of it in production or real applications, it **MUST** be thoroughly tested before implementation (use the code at your own risk).  
{: .prompt-danger }

> For TF6420 TwinCAT 3 Database Server, [BECKHOFF Infosys](https://infosys.beckhoff.com/content/1033/tf6420_tc3_database_server/index.html) contains comprehensive documentation. I highly encourage you to read it thoroughly!  
{: .prompt-danger }

## Instalation

TwinCAT Database Server is not installed by default with TwinCAT XAE/XAR. You must install it separately using the **TwinCAT Package Manager** for systems with build **4026 or higher**, or the **MSI (.exe installer)** for builds **4024 or lower**.  

### For >= 4026.0 systems
![Img](images/tf6420_post/tcpkg.png)
_TwinCAT Database Server location on TwinCAT Package Manager_

### For <= 4024.xx systems

[Link to TF6420 MSI Installer](https://www.beckhoff.com/en-en/products/automation/twincat/tfxxxx-twincat-3-functions/tf6xxx-connectivity/tf6420.html?)

![Img](images/tf6420_post/tf6420_msi.png)
_TwinCAT Database Server MSI Installer Website Location_

![Img](images/tf6420_post/executable.png)
_TwinCAT Database Server MSI Installer_

## TwinCAT Database Server Process

The TwinCAT Database Server service starts automatically along with the TwinCAT system on the control computer. It acts as the communication link between the PLC and the database. You can find it in the **Task Manager** under the **Processes** tab, as shown below:

![Img](images/tf6420_post/tf6420_process.png)
_TwinCAT Database Server Windows Process_
