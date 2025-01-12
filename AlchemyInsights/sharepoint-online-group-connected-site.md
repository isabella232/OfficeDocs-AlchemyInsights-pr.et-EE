---
title: Rühma lisamine SharePoint saidile
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318120"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Levinumad probleemid rühmaga ühendatud saidi loomisel SharePoint

1. Kui olete rühma ja selle ühendatud saidi kustutanud ja soovite luua teise sama URL-iga saidi, peate eelmise saidi jäädavalt eemaldama.

   - [SPO halduskesta allalaadimine](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Lisateavet PowerShelli kasutamist alustamise kohta leiate teemast SharePoint [Online Management Shelli kasutamine.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Eemaldage sait kustutatud saitidelt [cmdlet-käsu Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell abil. Rühmasaitide jäädavalt kustutamiseks on vaja Powershelli.

1. Kui loote rühmaga ühendatud saidi ja saate hoiatuse: sama pseudonüümiga rühm on juba **olemas,** kontrollige olemasolevaid rühmi [Microsoft 365 halduskeskus](https://admin.microsoft.com/AdminPortal/Home#/groups). Probleemi lahendamiseks kustutage olemasolev rühm, kui seda enam vaja pole, või looge sait, millele on määratud muu pseudonüüm.

1. Tänapäevaste rühmade loomiseks ja kasutamiseks on mitu võimalust, SharePoint.

   - Saate ühendada olemasolevad saidid Microsoft 365 rühmaga. Lisateavet leiate teemast [Ühendus Microsoft 365, kasutades SharePoint kasutajaliidest.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Rühmaga Microsoft 365 saidi loomiseks peate looma [meeskonnatöö saidi.](https://admin.microsoft.com/sharepoint)
