---
title: Luba Office 365 atp SharePoint, OneDrive ja Microsoft Teams
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
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964629"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Microsoft Defenderi Office 365 SharePoint Online'i, OneDrive ja Microsoft Teams

1. Avage ja https://protection.office.com logige sisse.
2. Valige **Ohuhalduspoliitika**  >    >  **seif Manused**.
3. Valige **Lülita Office 365 jaoks SharePoint, OneDrive** ja Microsoft Teams ja seejärel klõpsake nuppu **Salvesta**.
4. (Soovitatav) Käivitage üldadministraatori või SharePoint Online'i administraatorina [cmdlet-käsk Set-SPOTenant,](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) mille parameetri **DisallowInfectedFileDownload** väärtuseks on *seatud true*.
5. (Soovitatav) [Saate häälestada tuvastatud](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) failide teatised.

> [!NOTE]
> Microsoft Defender for Office 365 ei skanni kõiki SharePoint Online'is, OneDrive ega Microsoft Teams. Faile skannitakse asünkroonselt protsessi kaudu, mis kasutab ühiskasutus- ja külalistegevussündmusi ning nutikaid heuristika- ja ohusignaale pahatahtlike failide tuvastamiseks. Lisateavet [leiate teemast Microsoft Defender Office 365 SharePoint, OneDrive ja Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).