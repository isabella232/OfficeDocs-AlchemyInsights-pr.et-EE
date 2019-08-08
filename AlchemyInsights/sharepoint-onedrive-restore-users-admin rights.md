---
title: Tõrkeotsingu juurdepääs keelatud sõnumeid OneDrive äri saitide
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232519"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Tõrkeotsingu juurdepääs keelatud sõnumeid OneDrive äri saitide

See probleem tekib kõige sagedamini kui kasutaja kustutada ja uuesti luua sama Kasutaja turvasubjektinime (UPN). Uue konto loomiseks kasutatakse erinevaid PUID (passi kordumatu ID) väärtus. Kui kasutaja üritab pääseda saidikogumi või oma OneDrive, kasutajal on vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksusele (OU). See probleem võib tekkida, kui kasutajad on juba sisse logida SharePoint, siis kolis eri OU ja on SharePointi resynced, nad.

1. Selle probleemi lahendamiseks peaks taastama algse UPN koos artikli,[taastada kasutaja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)juhiseid.
2. Kui te ei saa taastada kasutaja tuleb eemaldada vana kasutaja OneDrive'i kaudu järgmiselt, [Eemalda kasutaja kasutaja info loendi]()abil. 
3. Kui see on tehtud, saate kontrollida kasutaja on admin õigused saidil OneDrive, järgides juhiseid [Lisa admin on kasutaja OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Õiguste kohta lisateabe saamiseks lugege artiklit, [mõistmise õigusetasemed SharePointi](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
