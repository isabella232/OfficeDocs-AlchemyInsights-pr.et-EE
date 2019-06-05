---
title: Võimaldada kasutajatele juurdepääs SharePointis või OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715208"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Võimaldada kasutajatele juurdepääs SharePointis või OneDrive

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">See probleem tekib kõige sagedamini kui kasutaja kustutada ja uuesti luua sama Kasutaja turvasubjektinime (UPN). Uue konto loomiseks kasutatakse erinevaid PUID (passi kordumatu ID) väärtus. Kui kasutaja üritab pääseda saidikogumi või oma OneDrive, kasutajal on vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksusele (OU). See probleem võib tekkida, kui kasutajad on juba sisse logida SharePoint, siis kolis eri OU ja on SharePointi resynced, nad.</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Selles küsimuses tuleks taastada algne UPN vajalike juhistega artiklis <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">taastada kasutaja Office 365.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Kui see on tehtud, saate kontrollida kasutaja on admin õigused saidil OneDrive, järgides juhiseid <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">lisada admin kasutaja OneDrive.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Õiguste kohta lisateabe saamiseks lugege artiklit, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">mõistmine õigusetasemed SharePointis.</a>&nbsp;</span></p>
