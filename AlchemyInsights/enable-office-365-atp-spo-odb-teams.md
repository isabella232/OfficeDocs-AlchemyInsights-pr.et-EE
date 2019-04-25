---
title: Office 365 ATP lubamine SharePoint, OneDrive ja Microsoft meeskonnad
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403029"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Luba Office 365 arenenud oht kaitse SharePoint Online, OneDrive ja Microsoft meeskonnad

1. Mine https://protection.office.com ja logige sisse.
2. Valida **ohu haldamise** > **poliitika** > **Safe Attachments**.
3. Valige **ATP SharePoint, OneDrive ja Microsoft meeskonnad sisse lülitada**ja klõpsake siis nuppu **Salvesta**.
4. (Soovitatav) Globaalne administraatori või SharePoint Online'i administraatori, käivitada [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet-käsu parameetri **DisallowInfectedFileDownload** väärtuseks *tõene*.
5. (Soovitatav) Tuvastatud failide [hoiatuste häälestus](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) .

> [!NOTE]
> ATP on nto skaneerida iga ühe faili SharePoint Online, OneDrive või Microsoft Teams. Asünkroonselt, kontrollitakse läbi protsessi, mis kasutab jagamine ja Külastajate tegevuse võistlusi, koos smart heuristics ja ohtu signaale pahatahtlike faile tuvastada faile. Vaadake [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).