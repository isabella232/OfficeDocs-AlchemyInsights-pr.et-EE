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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506914"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Lubage Office 365 täiustatud ohutõrje SharePoint Online ' i, OneDrive ja Microsoft Teamsi jaoks

1. https://protection.office.comsisse ja logige sisse.
2. Valige ohutaseme **halduse**  >  **poliitika**  >  **Turvalised manused**.
3. Valige **LÜLITA ATP SharePointi, OneDrive ja Microsoft Teams**ja seejärel klõpsake nuppu **Salvesta**.
4. Soovitatav Globaalne administraator või SharePoint Online ' i administraator, käivitage cmdlet [-käsu Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) koos parameetri **Disallowinfectedfiledownload** väärtuseks *True*.
5. Soovitatav [Seadistage](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tuvastatud failide teatised.

> [!NOTE]
> ATP aitab skannida iga faili SharePoint Online, OneDrive või Microsoft Teams. Faile skannitakse asünkroonselt protsessi kaudu, mis kasutab ühiskasutuse ja külalistegevuste sündmusi koos nutikate heuristika ja ohusignaalidega, et tuvastada pahatahtlikke faile. Vt [ATP SharePointi, OneDrive ' i ja Microsoft teamsi jaoks](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).