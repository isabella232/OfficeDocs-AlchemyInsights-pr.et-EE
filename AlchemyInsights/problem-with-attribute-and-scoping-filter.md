---
title: Atribuudi ja ulatuse filtri probleem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481364"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Atribuudi ja ulatuse filtri probleem

**Vastuolulised UPN-i väärtuste probleem**

Tööpäev AD kasutaja ettevalmistamine tööpäevaks AD kasutaja ettevalmistamine kuvab tõrketeate **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. Toiming nurjus, sest UPN-i väärtus, mis on ette nähtud lisamise/muutmisega, pole kogu metsa kordumatu. Tõrke üksikasjad: **CONSTRAINT_ATT_TYPE-userPrincipalName**.

**UserPrincipalName** väärtus, mille tööpäeva konnektor proovib määrata, kui loote ad User Account on juba olemas Target ad domeenis. See tähendab, et kas (1) kasutaja on juba olemas ja vastavad ID-d ei kontrollinud kasutaja või (2) UPN-i generatsiooni reegel genereeris vastuolulise väärtuse.

Siit leiate Soovitatavad eraldusvõime juhised.

Kui kasutaja on juba olemas ja vastava ID kontrollimisel ei õnnestunud linkida tööpäevade kontot Active Directory kontoga, siis kontrollige, kas vastaval tööpäeval ja REKLAAMIl on täpne vaste ID-atribuut (tavaliselt **employeeID**). Kui neil pole vastet, on vaja määrata andmete probleem. Kui EmployeeID tööpäeval on näiteks 001052 ja AD on 1052, siis ei saa kavandatav mootor kahe konto linkida ning proovib luua juba olemasoleva kasutaja. Lahendus sel juhul on muuta AD **EmployeeID** väärtust, et kaasata selle 001052.
Kui UPN-i genereeriv avaldis ei Genereeri kordumatut väärtust, kaaluge funktsiooni de-dubleerimise funktsiooni **SelectUniqueValue** abil iga kord ainulaadse väärtuse genereerimist.

**Tööpäeval AD kasutaja ettevalmistamine ei sea AD User Account Manageri atribuudi väärtust**

Tööpäev AD kasutaja ettevalmistamisel ei määra AD kasutajakontodele **halduri** atribuudi väärtust. Selle käitumise ilmnemisel on kaks võimalikku stsenaariumi.

1. Tööpäevade haldurit ei saa resolvida vastavale AD kasutajakontole, sest haldur pole ulatuses.
2. **Mitme ad-domeeni** stsenaariumi korral ei viibi haldur tööpäevas kasutajaga samas domeenis.

Probleemi lahendamiseks proovige järgmisi juhiseid.

1. Kui olete määranud filtrite määratlemine, siis kõigepealt kontrollige, kas haldur on rakendusalas ja kas see vastab ulatuse määramise klauslile. Kui haldur ei vasta filtri ulatuse filtrile, Muutke filtrit nii, et haldur oleks ka ettevalmistamisel.
2. Kui teil on mitu AD domeeni, on konnektoril teadaolevalt piiratud suutmatus lahendada domeenide halduri viiteid.

Lisateavet tööpäevade automaatseks ettevalmistamiseks konfigureerimise kohta leiate teemast [õpetus: tööpäevade automaatseks](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)ettevalmistamiseks konfigureerimine.













