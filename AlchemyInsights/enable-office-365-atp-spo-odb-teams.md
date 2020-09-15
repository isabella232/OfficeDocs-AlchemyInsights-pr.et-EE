---
title: Office 365 ATP lubamine SharePointi, OneDrive ' i ja Microsoft Teamsi jaoks
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709903"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online ' i, OneDrive ' i ja Microsoft Teamsi jaoks mõeldud Office 365 täiustatud ohu kaitse lubamine

1. Avage https://protection.office.com ja logige sisse.
2. Valige **ohustatud halduse**  >  **poliitika**  >  **Turvalised manused**.
3. Valige **Lülita SharePointi, OneDrive ' i ja Microsoft teamsi jaoks ATP**ja seejärel klõpsake nuppu **Salvesta**.
4. Soovitatav Globaalse administraatorina või SharePoint Online ' i administraatorina käivitage cmdlet [-käsk Set-spotenantiga](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) , mille parameeter **DisallowInfectedFileDownload** on seatud väärtusele *True*.
5. Soovitatav [Häälestage](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tuvastatud failide teatised.

> [!NOTE]
> ATP saab nSeadete skannida kõik failid SharePoint Online ' is, OneDrive ' is või Microsoft Teamsi. Failid skannitakse asünkroonselt kaudu, mis kasutab ühiskasutust ja Guest Activity üritusi, ning nutikad heuristilined ja ohud, et tuvastada pahatahtlikud failid. Lugege teemat [SharePointi, OneDrive ' i ja Microsoft teamsi ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).