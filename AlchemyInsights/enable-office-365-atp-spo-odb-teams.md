---
title: Office 365 ATP lubamine SharePointi, OneDrive ' i ja Microsofti meeskondade jaoks
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703422"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Lubage Office 365 täiustatud ohutõrje SharePoint Online ' i, OneDrive ja Microsoft Teamsi jaoks

1. sisse https://protection.office.com ja logige sisse.
2. Valige ohutaseme **halduse** > **poliitika** > **Turvalised manused**.
3. Valige **LÜLITA ATP SharePointi, OneDrive ja Microsoft Teams**ja seejärel klõpsake nuppu **Salvesta**.
4. Soovitatav Globaalne administraator või SharePoint Online ' i administraator, käivitage cmdlet [-käsu Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) koos parameetri **Disallowinfectedfiledownload** väärtuseks *True*.
5. Soovitatav [Seadistage](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tuvastatud failide teatised.

> [!NOTE]
> ATP aitab skannida iga faili SharePoint Online, OneDrive või Microsoft Teams. Faile skannitakse asünkroonselt protsessi kaudu, mis kasutab ühiskasutuse ja külalistegevuste sündmusi koos nutikate heuristika ja ohusignaalidega, et tuvastada pahatahtlikke faile. Vaata [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)seda.