---
title: Juurdepääs keelatud sõnumite tõrkeotsing
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503523"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Juurdepääs keelatud sõnumite OneDrive/SharePointi administreerimiskeskuses tõrkeotsing

Kui kuvatakse juurdepääsu keelamise teade, kui proovite SharePointi/OneDrive Admin kus, veenduge, et [määrata kasutaja litsentsi](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Kui kasutajal on litsentsi, samuti veenduge on [administraatoriroll](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) millele juurdepääs admin keskused.

See probleem võib ilmneda ka siis, kui kasutaja kustutada ja uuesti luua sama Kasutaja turvasubjektinime (UPN). Uue konto loomiseks kasutatakse erinevaid PUID (passi kordumatu ID) väärtus. Kui kasutaja üritab pääseda saidikogumi või oma OneDrive, kasutajal on vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksusele (OU). See probleem võib tekkida, kui kasutajad on juba sisse logida SharePoint, siis kolis eri OU ja on SharePointi resynced, nad.

Selle probleemi lahendamiseks peaks taastama algse UPN koos artikli, [taastada kasutaja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)juhiseid.

Märkus: Kui mitmele kasutajale, kellel juurdepääs puudub OneDrive'i või SharePointi Admin keskus, võib teenuse ajutise probleemi.  [Kontrollige teenuste seisundi armatuurlaud](https://portal.office.com/adminportal/home#/servicehealth).


