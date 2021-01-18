---
title: Domeeni teenuse konfigureerimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885219"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>AAD-DS-i või juurutust ei saa lubada

Azure AD Domain Service ' i (AAD-DS) probleemi lahendamiseks, mis ei ole lubatud või mida ei saa juurutada, tehke järgmist.

1. Kui kasutate juba olemasolevat virtuaalset võrku, märkige oma NSG reeglid, mis blokeerivad pordid, mida on vaja portaali AAD-DS sünkroonimiseks https://aka.ms/aadds-networking .
2. Vaadake, kas selles tõrkeotsingu juhendis on saadaval tõrketeade, et näha, kas teie tõrketeatele on vastatud  https://aka.ms/aadds-troubleshoot-enable .
3. Proovige juurutada Azure AD Domain Services uues virtuaalses võrgus.
4. Täitke juhised, kuidas juurutada AAD-DS: [AAD Domain Services loomine ja konfigureerimine](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Kui teil on Azure AD Domain Services juurutusega seotud probleeme, lugege teemat [AZURE ad Domain Services tõrkeotsing](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) levinud tõrgete lahendamiseks, mis aitavad teil asjad uuesti tööle saada. 

**AAD-DS-i ei saa keelata**

AAD-DS-i ei saa peatada. Kui soovite hallatava domeeni kasutamise lõpetada, tuleb see kustutada.
Hallatava domeeni kustutamiseks vaadake teemat [AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)' i kustutamine.



