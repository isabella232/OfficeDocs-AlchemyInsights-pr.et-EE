---
title: 126 Kas OWA-s ei leita postkasti saamist?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056486"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Kas teie postkastis ei leitud Outlooki veebirakendus?

Kui kasutate Outlooki veebirakendus postkasti ei leitud tõrke  tõttu, pole kontol, millega Outlooki veebirakendus-ga ühenduse loote, Exchange Online litsentsi ja seetõttu pole kontoga seotud ühtegi postkasti. Teie administraator saab teie kontole litsentsi määrata, järgides järgmisi juhiseid.

1. Avage [Microsoft 365 halduskeskus](https://portal.office.com/adminportal/home#/homepage) ja minge jaotises  Kasutajad jaotisse Aktiivsed kasutajad ja valige kasutaja, kes seda tõrget näeb. 

2. Avage avalehel jaotis Litsentsid  ja rakendused, valige sobiv  väärtus Asukoht ja määrake litsents, mis sisaldab Exchange Online (litsentsi üksikasjade määramiseks laiendage litsentsi). Kui olete lõpetanud, klõpsake nuppu **Salvesta muudatused.**

Mõnel juhul, kui litsents on juba kasutajakontole määratud, aitab litsentsi eemaldamine ja ümbermääramine probleemi lahendada ja seda süsteemis õigesti ette ettevalmistamise abil ette näha. 

- Kontrollige, kas teie M365 Exchange Online (ja muud, kui teil on) tellimused on praegused ja pole hiljuti aegunud.

Kui olete veendunud, et teie tellimus pole aegunud ja kasutajakontole on määratud kehtiv litsents, võib tellimuse ettevalmistamine võtta kuni 24 tundi, nii et peate võib-olla ootama, kuni probleem laheneks. Lisateavet leiate teemast [Litsentside määramine ja haldamine.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)