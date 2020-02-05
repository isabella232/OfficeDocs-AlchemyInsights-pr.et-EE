---
title: Rühma lisamine SharePointi saidile
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770347"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Probleemid rühma ühendatud saidi loomisel SharePointis

1. Mõne rühma ühendatud saidi loomisel või uuesti loomisel ilmnesid tavalised probleemid.
Kui olete kustutanud rühma ja selle ühendatud saidi ning soovite luua sama URL-iga mõne muu saidi, peate eelmise saidi jäädavalt eemaldama.

   - Lae alla [SPO Management shelli](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Lisateavet PowerShelli kohta alustamine, vaadake alustamine [SharePoint Online Management shelli](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Eemaldage saidi kustutatud saidid kasutades [Eemalda SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShelli cmdlet-käsu. Rühma saitide jäädavalt kustutamiseks on vaja PowerShelli.

1. Kui loote rühma ühendatud saidi ja kuvatakse hoiatus: **teine sama pseudonüümiga rühm on juba olemas**, kontrollige olemasolevaid rühmi [Office 365 alates administreerimiskeskusest](https://admin.microsoft.com/AdminPortal/Home#/groups). Probleemi lahendamiseks kustutage olemasolev rühm, kui see ei ole enam vajalik või luua saidi teise alias määratud.

1. On erinevaid viise, kuidas luua ja kasutada tänapäevaseid rühmi SharePointiga.

   - Saate ühendada olemasolevad saidid Office 365 rühma. Lisateavet leiate teemast [Office 365 rühma ühendamine SharePointi kasutajaliidese abil](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Office 365 rühma ühendatud saidi loomiseks peate looma [meeskonnatöö saidi](https://admin.microsoft.com/sharepoint).
