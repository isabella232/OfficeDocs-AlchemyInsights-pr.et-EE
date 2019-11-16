---
title: Tõrkeotsing juurdepääs keelatud sõnumid OneDrive for Business saidid
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766707"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Tõrkeotsing juurdepääs keelatud sõnumid OneDrive for Business saidid

See probleem ilmneb kõige sagedamini siis, kui kasutaja on kustutatud ja uuesti loodud sama kasutaja turvasubjektinimi (UPN). Uus konto on loodud, kasutades erinevaid PUID (Passporti kordumatu ID) väärtus. Kui kasutaja proovib pääseda saidikogumi või oma OneDrive, kasutaja on vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimine Active Directory organisatsiooniüksusele (OU). Kui kasutajad on juba SharePointi sisse logitud ja seejärel teisaldatakse teise OU ja uuesti SharePoint, need võivad ilmneda probleem.

1. Selle probleemi lahendamiseks peaksite taastama algse UPN juhiseid artiklis, [taastada kasutaja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Kui te ei saa taastada algne kasutaja peaks eemaldama vana kasutaja OneDrive saidi nende juhiste abil, [eemaldage kasutaja kasutajateabe loendist](). 
3. Pärast seda, kui see on tehtud, saate kontrollida kasutajal on administraatori õigused OneDrive saidi, järgides juhiseid [lisada admin kasutaja OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Õigusetasemete kohta lisateabe saamiseks lugege artiklit, [õigusetasemete mõistmine SharePointis](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
