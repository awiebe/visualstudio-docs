---
title: "Configure Firewall for Remote Debugging Dialog Box"
description: Read about the Configure Firewall for Remote Debugging dialog box, which appears when the Windows Firewall stops the debugger from receiving data over the network.
ms.date: "07/08/2022"
ms.topic: "ui-reference"
f1_keywords:
  - "vs.debug.firewallconfiguration"
dev_langs:
  - "CSharp"
  - "VB"
  - "FSharp"
  - "C++"
  - "JScript"
helpviewer_keywords:
  - "Configure Firewall for Remote Debugging dialog box"
  - "remote debugging, configuring firewalls"
  - "firewalls, configuring for remote debugging"
author: "mikejo5000"
ms.author: "mikejo"
manager: mijacobs
ms.subservice: debug-diagnostics
---
# Configure Firewall for Remote Debugging Dialog Box

This dialog box appears when the Windows Firewall blocks the debugger from receiving information over the network. To continue remote debugging, you must open a port in the firewall so the debugger can receive information.

> [!CAUTION]
> Opening a port in the Firewall may expose your machine to security threats that the Firewall is designed to block. Opening a port for remote debugging unblocks ports 4020 and 4021 in Visual Studio 2015. In other versions of Visual Studio, other port numbers are used. For more information, see [Remote Debugger Port Assignments](../debugger/remote-debugger-port-assignments.md). In addition, it allows the debugger to open additional ports. For more information, see [Configure the Windows Firewall for Remote Debugging](../debugger/configure-the-windows-firewall-for-remote-debugging.md).

## UIElement List
 **Cancel remote debugging**
 Cancels the remote debugging attempt. The security settings of your machine remain intact.

 **Unblock remote debugging from computers on the local network (subnet)**
 Enables remote debugging of machines on your local subnet. This may open vulnerabilities to machines on your local subnet, but the firewall continues to block information coming from outside the subnet.

 **Unblock remote debugging from any computer**
 Enables remote debugging of machines anywhere on the network. This setting is the least secure.

## See also

- [Debugger Security](../debugger/debugger-security.md)
- [Remote Debugging](../debugger/remote-debugging.md)
- [Debugging User Interface Reference](../debugger/debugging-user-interface-reference.md)