---
title: 618 kalendri ühiskasutuse poliitika
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684226"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Poliitika tõrge kalendri ühiskasutusse andmisel

1. Tehke vastavalt oma olukorrale ühte järgmistest.
    - Exchange Online ' iga ühenduse loomine Remote PowerShelli abil. Lisateavet leiate teemast [Exchange Online ' iga ühenduse loomine Remote PowerShelli abil](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Avage kohapealses serveris Exchange Management shell.
2. Määratakse kasutajale määratud ühiskasutuse poliitika. Selleks käivitage järgmine käsk ja pange tähele tagastatud poliitika.

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Värskendage kasutaja ühiskasutuse poliitikat. Selleks tehke järgmist.
    - Avage Exchange ' i halduskeskus.
    - Klõpsake nuppu **organisatsioon**ja seejärel topeltklõpsake poliitikat, mis on kasutajale määratud **iga ühiskasutuse**jaotises. See on poliitika, mis tagastati juhises 2.
    - Valige lehel ühiskasutuse reegel kalendri ühiskasutuse tase, mida soovite lubada jaotises **Määrake, millist teavet soovite ühiskasutusse anda**; Klõpsake nuppu **Salvesta**.

Lisateavet leiate järgmistest teemadest: ["poliitika ei luba sellel tasemel õiguste andmist ühele või mitmele adressaadile (s)" tõrge, kui kasutaja proovib kalendrit ühiskasutusse anda](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
