---
title: Rakenduse registreerimise omaniku probleemid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404455"
---
# <a name="app-registration-owner-issues"></a>Rakenduse registreerimise omaniku probleemid

Järgmised on saadaval meetodid subjektide lisamiseks rakenduse registreerimise omanikeks.

- Azure AD PowerShelli mooduli kasutamine –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Viide: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure'i CLI- `az ad app owner add`

    Viide: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS Graphi kasutamine

    Viide: [omaniku lisamine – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Azure AD portaali kasutamine – liikuge [lehele portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Valige > Owners > Add Owners (Omanikud)

**Kas te ei saa rakenduse registreerimiste teral oma rakendust vaadata, kuigi olete selle rakenduse omanik?**

Rakenduse omanik pole haldusroll. Kui säte [Piira juurdepääsu Azure AD haldusportaalile](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) on lubatud, saab ainult administraator rakendusi vaadata rakenduse registreerimise portaalis. Kui soovite, et omanik saaks rakendusi vaadata, keelake see säte (Määra see NO-ks) või määrake omanikule administraatori roll ainult konkreetse rakenduse jaoks. Selleks on aga vaja Azure AD Premium P2 litsentsi ja lubada [privilegeeritud identiteedihaldus.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
