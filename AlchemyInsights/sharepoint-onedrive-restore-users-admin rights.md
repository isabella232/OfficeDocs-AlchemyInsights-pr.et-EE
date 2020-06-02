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
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511180"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Tõrkeotsing juurdepääs keelatud sõnumid OneDrive for Business saidid

See probleem ilmneb kõige sagedamini siis, kui kasutaja on kustutatud ja uuesti loodud sama kasutaja turvasubjektinimi (UPN). Uus konto on loodud, kasutades erinevaid PUID (Passporti kordumatu ID) väärtus. Kui kasutaja proovib pääseda saidikogumi või oma OneDrive, kasutaja on vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimine Active Directory organisatsiooniüksusele (OU). Kui kasutajad on juba SharePointi sisse logitud ja seejärel teisaldatakse teise OU ja uuesti SharePoint, need võivad ilmneda probleem.

1. Selle probleemi lahendamiseks peaksite taastama algse UPN juhiseid artiklis, [taastada kasutaja Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Kui te ei saa taastada algne kasutaja peaks eemaldama vana kasutaja OneDrive saidi nende juhiste abil, [eemaldage kasutaja kasutajateabe loendist](). 
3. Pärast seda, kui see on tehtud, saate kontrollida kasutajal on administraatori õigused OneDrive saidi, järgides juhiseid [lisada admin kasutaja OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Õigusetasemete kohta lisateabe saamiseks lugege artiklit, [õigusetasemete mõistmine SharePointis](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
