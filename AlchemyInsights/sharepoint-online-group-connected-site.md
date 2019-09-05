---
title: Rühma lisamine SharePointi saidile
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750516"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Probleemid loomisel või rühma ühendatud saidid SharePoint Online

Rühma ühendatud saidi loomisel või uuesti loomisel ilmnesid mõned tavalised probleemid.

 Kui olete kustutanud rühma ja selle ühendatud saidi ning soovite luua sama URL-iga mõne muu saidi, peate eelmise saidi jäädavalt eemaldama.

Lae alla [SPO Management shelli](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Lisateavet PowerShelli kohta alustamine, vaadake alustamine [SharePoint Online Management shelli](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Eemaldage saidi kustutatud saidid kasutades [Eemalda SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShelli cmdlet-käsu.

Kui loote rühma ühendatud saidi ja kuvatakse hoiatus teine sama pseudonüümiga rühm on juba olemas, kontrollige olemasolevaid rühmi [Office 365 alates administreerimiskeskusest](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Probleemi lahendamiseks kustutage olemasolev rühm, kui see ei ole enam vajalik või luua saidi teise alias määratud.

On erinevaid viise, kuidas luua ja kasutada tänapäevaseid rühmi SharePointiga.

Saate ühendada olemasolevad saidid Office 365 rühma. Lisateabe saamiseks vaadake [Connect Office 365 rühma SharePointi kasutaja ineterface abil](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Office 365 rühma ühendatud saidi loomiseks peate looma meeskonnatöö saidi. Lisateavet leiate teemast [meeskonnatöö saidi loomine SharePointis](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

