---
title: Storage Migration Service known issues
description: Known issues and troubleshooting support for Storage Migration Service, such as how to collect logs for Microsoft Support.
author: nedpyle
ms.author: nedpyle
manager: siroy
ms.date: 11/07/2018
ms.topic: article
ms.prod: windows-server-threshold
ms.technology: storage
---
# Storage Migration Service known issues

This topic contains answers to known issues (KIs) when using [Storage Migration Service](overview.md) to migrate servers.

## <a name="collecting-logs"></a> How to collect log files when working with Microsoft Support

The Storage Migration Service contains event logs for the Orchestrator service and the Proxy Service. The urchestrator server always contains both event logs, and destination servers with the proxy service installed contain the proxy logs. These logs are located under:

- Application and Services Logs \ Microsoft \ Windows \ StorageMigrationService
- Application and Services Logs \ Microsoft \ Windows \ StorageMigrationService-Proxy

If you need to gather these logs for offline viewing or to send to Microsoft Support, there is an open source PowerShell script available on GitHub:

 [Storage Migration Service Helper](https://aka.ms/smslogs) 

Review the README for usage.

# Storage Migration Service known issues

When using the 1809 version of Windows Admin Center to manage a Windows Server 2019 orchestrator, you do not see the tool option for Storage Migration Service. 

The the Windows Admin Center Storage Migration Service extension is version-bound to only manage WIndows Server 2019 version 1809 or later operating systems. If you use it to manage older Windows Server operating systems or insider previews, the tool will not appear. This behavior is by design. 

To resolve, use or upgrade to Windows Server 2019 build 1809 or later.

## See also

- [Storage Migration Service overview](overview.md)