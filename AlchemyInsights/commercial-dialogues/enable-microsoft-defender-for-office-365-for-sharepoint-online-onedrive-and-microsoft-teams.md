---
title: Microsoft Defenderi lubamine Office 365 for SharePoint Online ' i, OneDrive ' i ja Microsoft Teamsi jaoks
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744113"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Microsoft Defenderi lubamine Office 365 for SharePoint Online ' i, OneDrive ' i ja Microsoft Teamsi jaoks

1. Logige sisse oma üldadministraatori või administraatori mandaadiga, logige sisse teenusekomplekti [Office 365 turbe-ja vastavuskontrolli keskusse](https://protection.office.com/).
2. Valige vasakpoolsel paanil **ohu haldus** ja seejärel valige **poliitika**  >  [Turvalised manused](https://protection.office.com/safeattachment).
3. Valige **Lülita Microsoft Defenderi jaoks ette Office 365 SharePointi, OneDrive ' i ja Microsoft teamsi** jaoks ning seejärel valige **Salvesta**.
    > [!TIP]
    >
    > - Globaalse administraatorina või SharePoint Online ' i administraatorina käivitage järgmine PowerShelli cmdlet, mille **DisallowInfectedFileDownload** parameeter on seatud väärtusele *True*: [Set-spotenantiga](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Teatiste häälestamine tuvastatud failide jaoks](https://go.microsoft.com/fwlink/?linkid=2092110)

Lisateavet leiate teemast [Microsoft Defender for Office 365 SharePointi, OneDrive ' i ja Microsoft teamsi](https://go.microsoft.com/fwlink/?linkid=2092041)jaoks.
