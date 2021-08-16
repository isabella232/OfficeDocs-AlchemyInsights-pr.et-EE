---
title: Microsoft Defenderi Office 365 SharePoint Online'i, OneDrive ja Microsoft Teams
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
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058862"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Microsoft Defenderi Office 365 SharePoint Online'i, OneDrive ja Microsoft Teams

1. Logige üldadministraatori või turbeadministraatori identimisteabe abil [sisse Office 365 turbe- ja vastavuskeskusesse.](https://protection.office.com/)
2. Valige **vasakul paanil** Ohuhaldus ja seejärel poliitika **ja**  >  [seif manused](https://protection.office.com/safeattachment).
3. Valige **Lülita microsoft Defender Office 365 jaoks SharePoint, OneDrive ja Microsoft Teams** ja seejärel valige **Salvesta**.
    > [!TIP]
    >
    > - Käivitage üldadministraatori või SharePoint Online'i administraatorina järgmine PowerShelli cmdlet-käsk, mille parameetri **DisallowInfectedFileDownload** väärtuseks on *seatud true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Tuvastatud failide teatiste seadistamine](https://go.microsoft.com/fwlink/?linkid=2092110)

Lisateavet leiate teemast [Microsoft Defender for Office 365 for SharePoint, OneDrive ja Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
