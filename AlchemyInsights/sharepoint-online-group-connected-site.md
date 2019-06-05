---
title: Rühma lisamine SharePointi saidil
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719478"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Luua rühma ühendatud saidi SharePoint Online

<p><strong>On ühiseid teemasid kui ühendatud loomine või uuesti luua rühma saidi paar.&nbsp;</strong></p>  <p>1.Kui rühma ja sellega seotud saidi kustutanud ja soovite luua teisele saidile sama URL-iga, peate eelmisest jäädavalt eemaldada.</p>  <ul>  <li>Lae <a title="SPO halduskestas" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management shelli</a> - PowerShelliga alustamise kohta leiate teemast <a title="alustamine SharePoint Online halduskestas" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Alustamine: SharePoint Online Management shelli</a>. <br /><br /></li>  <li>Eemaldada saidi kustutada saidid kasutades on <a title="Eemalda-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Eemalda SPODeletedSite</a> PowerShelli cmdlet-i.</li>  </ul>  <p>Kui rühma ühendatud saidi loomisel kuvatakse hoiatus <strong>"teine rühm on sama pseudonüüm on juba olemas"</strong>, kontrollige olemasolevaid rühmad on <a title="Office 365 halduskeskuse kaudu" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 halduskeskuse kaudu</a>. Probleemi lahendamiseks, olemasoleva rühma kustutada, kui see ei ole enam vajalik või luua saidi eri alias määratud.&nbsp;</p>  <p><strong>On erinevaid viise, kuidas luua ja kasutada kaasaegseid sõprade SharePointiga.&nbsp;</strong></p>  <ol>  <li>Interneti Office 365 rühma olemasolevatel saitidel. Lisateavet leiate teemast <a title="ühendust Office 365 rühma, kasutades SharePointi kasutaja ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Ühendust Office 365 rühma, kasutades SharePointi kasutaja ineterface</a>.</li>  <li>Office 365 rühma ühendatud saidi loomiseks peate luua meeskonnatöö veebisaidi. Lisateavet leiate teemast <a title="SharePointi meeskonnatöö saidi loomine" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Meeskonnatöö saidi loomine SharePointi.</a></li>  </ol>

