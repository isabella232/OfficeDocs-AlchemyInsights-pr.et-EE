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
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951129"
---
# <a name="app-registration-owner-issues"></a>Rakenduse registreerimise omaniku probleemid

Järgmised on saadaval meetodid subjektide lisamiseks rakenduse registreerimise omanikeks.

- Azure AD PowerShelli mooduli kasutamine –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Viide: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure'i CLI- `az ad app owner add`

    Viide: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Ms Graph -

    Viide: [omaniku lisamine – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Azure AD portaali kasutamine – liikuge [lehele portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Valige > Owners > Add Owners (Omanikud)

**Kas te ei saa rakenduse registreerimiste teral oma rakendust vaadata, kuigi olete selle rakenduse omanik?**

Rakenduse omanik pole haldusroll. Kui säte [Piira juurdepääsu Azure AD haldusportaalile](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) on lubatud, saab ainult administraator rakendusi vaadata rakenduse registreerimise portaalis. Kui soovite, et omanik saaks rakendusi vaadata, keelake see säte (Määra see NO-ks) või määrake omanikule administraatori roll ainult konkreetse rakenduse jaoks. Selleks on siiski vaja Azure AD Premium P2 litsentsi ja [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
