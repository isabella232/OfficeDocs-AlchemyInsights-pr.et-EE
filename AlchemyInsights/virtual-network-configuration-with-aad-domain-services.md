---
title: Virtuaalne konfiguratsioon AAD Domain Services ' i abil
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
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885206"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuaalne konfiguratsioon AAD Domain Services ' i abil

AAD Domain Services virtuaalne konfiguratsioon hõlmab järgmisi toiminguid. 

1. Domeeni tervise kontrollimine Azure ' i portaalis https://aka.ms/aadds-health
2. NSG kontrollimine reeglite jaoks, mis blokeerivad pordid, mida on vaja Azure AD Domain Services ' is sünkroonimiseks portaalis https://aka.ms/aadds-networking
3. Tagab, et teie Virtual Network on juurutatud sama Azure ' i piirkonnas Azure AD Domain Services hallatava domeeniga.
4. Tagamaks, et teil pole olemasolevat domeeni, millel on sama domeeninimi, mis on saadaval ka virtuaalses võrgus.

Lisateavet selle kohta, kuidas Azure Virtual Network for SharePoint Virtual Network for AAD Domain Services toetamise kohta lisateabe saamiseks lugege teemat [Virtual Network tasu](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)

