---
title: Tõrkeotsing juurdepääs keelatud sõnumid OneDrive for Business saidid
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051601"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Tõrkeotsing juurdepääs keelatud sõnumid OneDrive for Business saidid

See probleem ilmneb kõige sagedamini siis, kui kasutaja on kustutatud ja uuesti loodud sama kasutaja turvasubjektinimi (UPN). Uus konto on loodud, kasutades erinevaid PUID (Passporti kordumatu ID) väärtus. Kui kasutaja proovib pääseda saidikogumi või oma OneDrive, kasutaja on vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimine Active Directory organisatsiooniüksusele (OU). Kui kasutajad on juba SharePointi sisse logitud ja seejärel teisaldatakse teise OU ja uuesti SharePoint, need võivad ilmneda probleem.

1. Selle probleemi lahendamiseks peaksite taastama algse UPN juhiseid artiklis, [taastada kasutaja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Kui te ei saa taastada algne kasutaja peaks eemaldama vana kasutaja OneDrive saidi nende juhiste abil, [eemaldage kasutaja kasutajateabe loendist](). 
3. Pärast seda, kui see on tehtud, saate kontrollida kasutajal on administraatori õigused OneDrive saidi, järgides juhiseid [lisada admin kasutaja OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Õigusetasemete kohta lisateabe saamiseks lugege artiklit, [õigusetasemete mõistmine SharePointis](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
