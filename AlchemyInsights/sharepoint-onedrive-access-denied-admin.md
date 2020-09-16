---
title: Accessi keelatud sõnumite tõrkeotsing
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767658"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>SharePointi/OneDrive ' i administreerimiskeskuses keelatud sõnumite juurdepääsu tõrkeotsing

Kui saate SharePointi/OneDrive ' i administreerimiskeskuse sirvimisel juurdepääsu keelamise teate, veenduge, et [määrate kasutajale litsentsi](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Kui kasutajal on litsents, peate veenduma, et neile määratakse administraatori keskustele juurdepääsuks [administraatori roll](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) .

See probleem võib ilmneda ka siis, kui kasutaja kustutatakse ja luuakse uuesti sama kasutaja põhinimega (UPN). Uue konto loomisel kasutatakse mõnda muud PUID (passi kordumatu ID). Kui kasutaja proovib juurde pääseda saidikogumile või nende OneDrive ' i, on kasutajal vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksuse (OU) abil. Kui kasutajad on juba SharePointi sisse loginud ja seejärel teisaldatakse need teise OU ja sünkroonitakse SharePointiga, võivad nad seda probleemi kogeda.

Selle probleemi lahendamiseks peaksite taastama algse UPN-i artikli juhistega, [taastama kasutaja Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Märkus: kui OneDrive ' i või SharePointi halduskeskus pole saadaval mitmele kasutajale, kellel oli varem juurdepääs, võib tegemist olla ajutise teenuse probleemiga.  [Kontrollige teenuse tervise armatuurlauda](https://portal.office.com/adminportal/home#/servicehealth).


