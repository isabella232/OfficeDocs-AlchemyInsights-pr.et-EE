---
title: Oma asutuse meilisõnumite otsimine ja kustutamine
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524280"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Oma asutuse meilisõnumite otsimine ja kustutamine

Tehke järgmist.

1. Kui te pole üldadministraator, saate sõnumite otsimiseks lisada oma konto e- **juurdluse halduri rollirühma** või **vastavuse otsingu juhtimise rollile**. Sõnumite kustutamiseks peate liituma **organisatsiooni juhtimise rollirühma** või **otsingu ja likvideerimise rolliga**. Nende rollide kasutusõigused määratakse [turbe & täitmise keskuses.](https://protection.office.com)
2. [Saate luua sisu otsimise](https://docs.microsoft.com/office365/securitycompliance/content-search) , et leida sõnum, mille soovite kustutada.
3. [Looge ühendus turbe & vastavuse keskusega PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Kui kasutate MFA-i, lugege järgmisi juhiseid: [ühenduse loomine turbe & ühilduvuse keskusega PowerShelli abil mitme teguriga autentimine](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Kustutage sõnum: Käivitage `New-ComplianceSearchAction` cmdlet-käsk, et sõnum kustutada. Kustutatud sõnumid teisaldatakse kasutaja taastatavate üksuste kausta. Näites toodud juhised leiate artiklist [3: sõnumi kustutamine.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
