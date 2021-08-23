---
title: Rakenduses "Rakenduse juhtimine" ei kuvata minu rakendust
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454538"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Rakenduses "Rakenduse juhtimine" ei kuvata minu rakendust

Kui teie rakendust ei kuvata rakenduses Juhtimine, kontrollige järgmist.

1. Avage [Azure AD](https://aad.portal.azure.com/) ja otsige rakenduse ID üles, otsides lehe Ülevaade ülaribalt rakenduse nime.

1. Access Graph Explorer ja otsige teenusesubjektis rakenduse ID-d, kasutades seda päringut ja asendades vastava <appId> rakenduse ID-ga: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Kui tulemeid ei tagastata, otsige rakenduse ID-d selle päringu abil ja asendage see vastava rakenduse <appId> ID-ga: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Kui teil on päringuga probleeme, lugege teemat [Tugiteenused](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Lisateavet rakendusehalduse rakenduste kohta leiate teemast Teave nähtavuse [ja ülevaadete kohta.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Lisateavet rakenduste vaatamise kohta leiate teemast [Rakenduste vaatamine.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
