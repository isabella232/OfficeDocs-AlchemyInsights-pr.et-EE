---
title: Luba seif-, SharePoint-, OneDrive- ja Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332375"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Luba seif-, SharePoint-, OneDrive- ja Microsoft Teams

1. Avage üldadministraatori või turbeadministraatori identimisteabe Microsoft 365 Defender ja seejärel avage jaotises Poliitikad & reeglid <https://security.microsoft.com>  \>  \> **Ohupoliitikad seif** **Manused**

   Otse lehele Manused **seif** avanemiseks kasutage nuppu <https://security.microsoft.com/safeattachmentv2> .

2. Klõpsake **seif Manused** nuppu **Üldsätted.**
3. Valige kuvataval hüpikmenüüs käsk **Lülita Microsoft Defender Office 365 SharePoint, OneDrive ja Microsoft Teams** ja seejärel valige **Salvesta**.

    **Näpunäide.** Järgmiste toimingute abil saate seif, SharePoint OneDrive ja Microsoft Teams.
    - Et kasutajad ei saa pahatahtlikke faile alla laadida, kasutage `$true` SharePoint PowerShelli **[cmdlet-käsu Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** parameetri *DisallowInfectedFileDownload* väärtust. Lisateavet leiate teemast SharePoint [PowerShelli kasutamine, et takistada kasutajatel pahatahtlikke faile alla laadida.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Tuvastatud failidele teatisepoliitika loomine](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Lisateavet leiate teemast [seif manused Office 365 SharePoint, OneDrive ja Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
