---
title: Microsoft Defender Antivirus compatibility with Microsoft Defender ATP
description: Learn about how Windows Defender works with Microsoft Defender ATP and how it functions when a third-party antimalware client is used.  
keywords: windows defender compatibility, defender, microsoft defender atp
search.product: eADQiWindows 10XVcnh
search.appverid: met150
ms.prod: w10
ms.mktglfcycl: deploy
ms.sitesec: library
ms.pagetype: security
ms.author: macapara
author: mjcaparas
ms.localizationpriority: medium
manager: dansimp
audience: ITPro
ms.collection: M365-security-compliance 
ms.topic: conceptual
ms.date: 04/24/2018
---

# Microsoft Defender Antivirus compatibility with Microsoft Defender ATP

[!INCLUDE [Microsoft 365 Defender rebranding](../../includes/microsoft-defender.md)]


**Applies to:**


- Windows Defender
- [Microsoft Defender for Endpoint](https://go.microsoft.com/fwlink/p/?linkid=2146631)



>Want to experience Defender for Endpoint? [Sign up for a free trial.](https://www.microsoft.com/microsoft-365/windows/microsoft-defender-atp?ocid=docs-wdatp-defendercompat-abovefoldlink)

The Microsoft Defender for Endpoint agent depends on Microsoft Defender Antivirus for some capabilities such as file scanning.

>[!IMPORTANT]
>Defender for Endpoint does not adhere to the Microsoft Defender Antivirus Exclusions settings. 

You must configure Security intelligence updates on the Defender for Endpoint devices whether Microsoft Defender Antivirus is the active antimalware or not. For more information, see [Manage Microsoft Defender Antivirus updates and apply baselines](../microsoft-defender-antivirus/manage-updates-baselines-microsoft-defender-antivirus.md).

If an onboarded device is protected by a third-party antimalware client, Microsoft Defender Antivirus on that endpoint will enter into passive mode.

Microsoft Defender Antivirus will continue to receive updates, and the *mspeng.exe* process will be listed as a running a service, but it will not perform scans and will not replace the running third-party antimalware client.

The Microsoft Defender Antivirus interface will be disabled, and users on the device will not be able to use Microsoft Defender Antivirus to perform on-demand scans or configure most options.

For more information, see the [Microsoft Defender Antivirus and Defender for Endpoint compatibility topic](../microsoft-defender-antivirus/microsoft-defender-antivirus-compatibility.md).
