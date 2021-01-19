---
title: Domeenikontroller
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900872"
---
# <a name="domain-controller"></a>Domeenikontroller

**AAD-DS-i või juurutust ei saa lubada**

Azure AD Domain Service ' i (AAD-DS) probleemi lahendamiseks, mis ei ole lubatud või mida ei saa juurutada, tehke järgmist.

1. Kui kasutate juba olemasolevat virtuaalset võrku, märkige oma NSG reeglid, mis blokeerivad pordid, mida on vaja portaali AAD-DS sünkroonimiseks https://aka.ms/aadds-networking .
2. Vaadake, kas selles tõrkeotsingu juhendis on saadaval tõrketeade, et näha, kas teie tõrketeatele on vastatud  https://aka.ms/aadds-troubleshoot-enable .
3. Proovige juurutada Azure AD Domain Services uues virtuaalses võrgus.
4. Täitke juhised selle kohta, kuidas juurutada AAD-DS-i, mis on saadaval aadressil [juhendaja AZURE ad Domain Services loomiseks](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Kui teil on Azure AD Domain Services juurutusega seotud probleeme, lugege teemat [AZURE ad Domain Services tõrkeotsing](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) levinud tõrgete lahendamiseks, mis aitavad teil asjad uuesti tööle saada. 

**AAD-DS-i ei saa keelata**

AAD-DS-i ei saa peatada. Kui soovite hallatava domeeni kasutamise lõpetada, tuleb see kustutada.

Kui teil tekib probleeme, Lahendage levinud tõrketeated ja seotud tõrkeotsingu toimingud, et aidata teil asju uuesti käivitada, lugege teemat [Azure Active Directory Domain Services tõrkeotsing](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
