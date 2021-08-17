---
title: Juurdepääsu keelanud sõnumite tõrkeotsing
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085224"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>SharePointis/OneDrive halduskeskuses juurdepääsu keelanud sõnumite tõrkeotsing

Kui sharepointi või OneDrive halduskeskuseni sirvimisel kuvatakse juurdepääs keelatud sõnumile, siis veenduge, et määrate [kasutajale litsentsi.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Kui kasutajal on litsents, peaksite veenduma, et talle määratakse administraatori [roll, mis](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) pääseb juurde halduskeskustele.

See probleem võib ilmneda ka siis, kui kasutaja kustutatakse ja luuakse uuesti sama kasutajasubjektinimega (UPN). Uue konto loomiseks kasutatakse erinevat PUID-i (Passport Unique ID) väärtust. Kui kasutaja proovib juurde pääseda saidikogumile või tema OneDrive, on kasutajal vale PUID. Teine stsenaarium hõlmab kataloogisünkroonimist Active Directory organisatsiooniüksusega (OU). Kui kasutajad on juba SharePoint sisse loginud ja seejärel teisaldatakse teise OU-sse ja sünkroonitakse SharePoint, võib see probleem ilmneda.

Selle probleemi lahendamiseks peaksite algse UPN-i taastama artiklis "Kasutaja taastamine [Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Märkus. Kui OneDrive või SharePoint pole saadaval mitmele kasutajale, kellel oli varem juurdepääs, võib esineda ajutine teenuseprobleem.  [Kontrollige teenuse seisundi armatuurlauda.](https://portal.office.com/adminportal/home#/servicehealth)


