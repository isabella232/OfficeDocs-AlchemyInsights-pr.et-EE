---
title: Juurdepääs keelatud sõnumite tõrkeotsing
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505375"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Juurdepääs keelatud sõnumite tõrkeotsing SharePointi/OneDrive ' i administreerimiskeskuses

Kui teil on juurdepääs keelatud sõnumi sirvimisel SharePointi/OneDrive ' i administreerimiskeskus, veenduge, et [määrata litsentsi kasutajale](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Kui kasutajal on litsents, peaksite ka veenduma, et neile [määratakse administraatoriroll](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , mis pääseb juurde administreerimiskeskustele.

See probleem võib ilmneda ka siis, kui kasutaja on kustutatud ja uuesti loodud sama kasutaja turvasubjektinimi (UPN). Uus konto on loodud, kasutades erinevaid PUID (Passporti kordumatu ID) väärtus. Kui kasutaja proovib pääseda saidikogumi või oma OneDrive, kasutaja on vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimine Active Directory organisatsiooniüksusele (OU). Kui kasutajad on juba SharePointi sisse logitud ja seejärel teisaldatakse teise OU ja uuesti SharePoint, need võivad ilmneda probleem.

Selle probleemi lahendamiseks peaksite taastama algse UPN juhiseid artiklis, [taastada kasutaja Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Märkus: kui OneDrive või SharePointi administreerimiskeskus pole saadaval mitmele kasutajale, kellel oli varem juurdepääs, võib olla ajutine teenuse probleem.  [Kontrollige teenuse tervise armatuurlauda](https://portal.office.com/adminportal/home#/servicehealth).


