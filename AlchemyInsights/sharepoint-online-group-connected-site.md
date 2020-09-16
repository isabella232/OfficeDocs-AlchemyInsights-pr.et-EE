---
title: Rühma lisamine SharePointi saidile
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771195"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Probleemid rühma ühendatud saidi loomisel rakenduses SharePoint

1. Mõned levinud probleemid, mis tekkisid rühma ühendatud saidi loomisel või uuesti loomisel.
Kui olete rühma ja selle ühendatud saidi kustutanud ning soovite luua sama URL-iga mõne teise saidi, peate eelmise saidi jäädavalt eemaldama.

   - Laadi alla [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Lisateavet PowerShelli kasutamise kohta leiate teemast [SharePoint Online ' i haldamise kestaga alustamine](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Eemaldage sait kustutatud saitidelt, kasutades SPODeletedSite PowerShelli cmdlet [-](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) käsku. Rühma saitide jäädavalt kustutamiseks on vaja PowerShelli.

1. Kui loote rühma ühendatud saiti ja saadate hoiatuse: **teine sama pseudonüümiga rühm on juba olemas**, vaadake olemasolevaid rühmi [Microsoft 365 halduskeskus](https://admin.microsoft.com/AdminPortal/Home#/groups). Probleemi lahendamiseks kustutage olemasolev rühm, kui seda pole enam vaja, või looge sait mõne muu määratud pseudonüümiga.

1. SharePointi jaoks on moodsate rühmade loomiseks ja kasutamiseks mitu võimalust.

   - Saate ühendada olemasolevad saidid Microsoft 365 rühmaga. Lisateavet leiate teemast [Microsoft 365 rühma ühendamine SharePointi kasutajaliidese abil](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Microsoft 365 rühmaga ühendatud saidi loomiseks peate looma [meeskonnatöö saidi](https://admin.microsoft.com/sharepoint).
