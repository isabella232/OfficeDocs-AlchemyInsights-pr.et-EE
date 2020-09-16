---
title: Teave Yammeri identiteedi kohta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664166"
---
# <a name="about-identity-in-yammer"></a>Teave Yammeri identiteedi kohta

Identiteediga seotud probleemide vältimiseks soovitame kõigil võrkudel teha järgmisi toiminguid.

1. Office 365 identiteedi jõustamine pärast seda, kui Microsoft 365 on Azure AD kasutajatele ette valmistanud, veenduge, et kõik kasutajad logivad sisse oma peamise Microsoft 365 konto abil. Lisateavet leiate teemast [Office 365 identiteedi jõustamine Yammeri kasutajate jaoks](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolideerida mitu Yammeri võrku. Pärand Yammeri konfiguratsioonid võimaldavad mitu Yammeri võrku ühendada ühe rentniku jaoks. Lisateavet leiate teemast [võrgu migreerimine – mitme Yammeri võrgu konsolideerimine](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Soovi korral saate Yammeri kasutajatele blokeerida ka Yammeri litsentsimise, kui neil pole litsentsi. Lisateavet leiate teemast [Yammeri kasutajate litsentside haldamine Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Lõpetuseks auditeerige vanemate Yammeri võrkude kasutajate loendit ja katkestage pärandi kasutajad. Soovitatav on kasutajate kustutamise asemel peatada (desaktiveerida), kuna kustutamine on pöördumatu. Lisateavet leiate teemast [Yammeri kasutajate auditeerimine Office 365 ühendatud võrkudes](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) ja [kasutajate eemaldamine](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Yammeri konfigureerimine nende juhiste abil saate ka oma Yammeri võrgu konfigureerida Microsoft 365-i emakeelena režiimis. Lisateavet leiate teemast [Yammeri võrgu konfigureerimine Microsoft 365-i emakeelena režiimis](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).