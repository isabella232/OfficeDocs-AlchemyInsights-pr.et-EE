---
title: OneDrive for Businessi saitidele juurdepääsu keelamise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670612"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>OneDrive for Businessi saitidele juurdepääsu keelamise tõrkeotsing

See probleem ilmneb kõige sagedamini siis, kui kasutaja kustutatakse ja luuakse uuesti sama kasutaja põhinimega (UPN). Uue konto loomisel kasutatakse mõnda muud PUID (passi kordumatu ID). Kui kasutaja proovib juurde pääseda saidikogumile või nende OneDrive ' i, on kasutajal vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksuse (OU) abil. Kui kasutajad on juba SharePointi sisse loginud ja seejärel teisaldatakse need teise OU ja sünkroonitakse SharePointiga, võivad nad seda probleemi kogeda.

1. Selle probleemi lahendamiseks peate taastama algse UPN-i artikli juhistega, [taastama kasutaja Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Kui te ei saa algset kasutajat taastada, peate vana kasutaja nende juhiste abil OneDrive ' i saidilt eemaldama, [eemaldage kasutaja kasutaja teabe loendist](). 
3. Kui see on tehtud, saate kontrollida, kas kasutajal on OneDrive ' i saidi administraatori õigused, järgides juhiseid [kasutaja OneDrive ' i jaoks administraatorile lisamiseks](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Lisateavet õiguste tasemete kohta leiate artiklist, [õiguste tasemete mõistmine SharePointis](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
