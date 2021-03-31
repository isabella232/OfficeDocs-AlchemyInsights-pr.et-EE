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
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426658"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Kas Outlooki veebirakenduses ei leitud postkasti tõrkeid?

Kui kasutate Outlooki veebirakendust ja tõrketeadet  postkasti ei leitud, pole kontol, mida kasutasite Outlooki veebirakendusega ühenduse loomiseks, Exchange Online'i litsentsi ja seetõttu pole kontoga seotud ühtegi postkasti. Teie administraator saab teie kontole litsentsi määrata, järgides järgmisi juhiseid.

1. Avage [Microsoft 365 halduskeskus](https://portal.office.com/adminportal/home#/homepage)  ja avage  jaotises Kasutajad jaotis Aktiivsed kasutajad ja valige kasutaja, kes seda tõrget näeb.

2. Avage avalehel jaotis Litsentsid **ja** rakendused, valige sobiv  väärtus Asukoht ja määrake litsents, mis sisaldab Exchange Online'i (litsentsi üksikasjade määramiseks laiendage litsentsi). Kui olete lõpetanud, klõpsake nuppu **Salvesta muudatused.**

Mõnel juhul, kui litsents on juba kasutajakontole määratud, aitab litsentsi eemaldamine ja ümbermääramine probleemi lahendada ja seda süsteemis õigesti ette ettevalmistamise abil ette näha. 

- Kontrollige, kas teie M365 Exchange Online'i (ja muud, kui teil on) tellimused on praegused ja pole hiljuti aegunud.

Kui olete veendunud, et teie tellimus pole aegunud ja kasutajakontole on määratud kehtiv litsents, võib tellimuse ettevalmistamine võtta kuni 24 tundi, nii et peate võib-olla ootama, kuni probleem laheneks. Lisateavet leiate teemast [Litsentside määramine ja haldamine.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)