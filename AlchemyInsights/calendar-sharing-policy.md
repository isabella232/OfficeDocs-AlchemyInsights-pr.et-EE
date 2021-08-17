---
title: 618 Kalendri ühiskasutuse poliitika
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091598"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Poliitikatõrge kalendri ühiskasutusel

1. Tehke vastavalt olukorrale ühte järgmistest.
    - Ühendus Exchange Online remote PowerShelli abil. Lisateavet leiate teemast Ühendus [Exchange Online remote PowerShelli abil.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - Avage kohapealne server halduskesta Exchange.
2. Määratlege kasutajale määratud ühiskasutuspoliitika. Selleks käivitage järgmine käsk ja pange tähele, et poliitika on tagastatud.

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Värskendage kasutaja ühiskasutuspoliitikat. Selleks tehke järgmist.
    - Avage Exchange halduskeskus.
    - Klõpsake **nuppu** Organisatsioon ja seejärel topeltklõpsake jaotises Üksik ühiskasutus kasutajale määratud **poliitikat.** See on poliitika, mis tagastati 2. juhises.
    - Valige lehel Ühiskasutusreegel kalendri ühiskasutuse tase, mille soovite lubada jaotises **Määrake, millist teavet soovite ühiskasutusse anda.** klõpsake **nuppu Salvesta**.

Lisateavet leiate teemast "Poliitika ei luba sellel tasemel õiguste andmist ühele või mitmele adressaadile", kui kasutaja proovib [kalendrit ühiskasutusse anda.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
