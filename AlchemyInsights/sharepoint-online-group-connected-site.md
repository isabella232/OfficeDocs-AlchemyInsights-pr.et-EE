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
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507843"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="b560b-102">Probleemid, kui luua või rühma ühendatud saitidel SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b560b-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="b560b-103">On ühiseid teemasid kui ühendatud loomine või uuesti luua rühma saidi paar.</span><span class="sxs-lookup"><span data-stu-id="b560b-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="b560b-104">Kui rühma ja sellega seotud saidi kustutanud ja soovite luua teisele saidile sama URL-iga, peate eelmisest jäädavalt eemaldada.</span><span class="sxs-lookup"><span data-stu-id="b560b-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="b560b-105">Lae [SPO halduskestas](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="b560b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="b560b-106">Rohkem infot kuidas alustada PowerShelli abil, vaadake [SharePoint Online halduskesta alustamine](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="b560b-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="b560b-107">Eemalda saidi kustutada saidid kasutades [Eemalda-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShelli cmdlet-i.</span><span class="sxs-lookup"><span data-stu-id="b560b-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="b560b-108">Kui rühma ühendatud saidi loomisel kuvatakse hoiatus, teine rühm sama pseudonüüm on juba olemas, kontrollige [Office 365 halduskeskuse kaudu](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)olemasolevatesse gruppidesse.</span><span class="sxs-lookup"><span data-stu-id="b560b-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="b560b-109">Probleemi lahendamiseks, olemasoleva rühma kustutada, kui see ei ole enam vajalik või luua saidi eri alias määratud.</span><span class="sxs-lookup"><span data-stu-id="b560b-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="b560b-110">On erinevaid viise, kuidas luua ja kasutada kaasaegseid sõprade SharePointiga.</span><span class="sxs-lookup"><span data-stu-id="b560b-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="b560b-111">Interneti Office 365 rühma olemasolevatel saitidel.</span><span class="sxs-lookup"><span data-stu-id="b560b-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="b560b-112">Lisateavet leiate teemast [ühendamine Office 365 rühma, kasutades SharePointi kasutaja ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="b560b-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="b560b-113">Office 365 rühma ühendatud saidi loomiseks peate luua meeskonnatöö veebisaidi.</span><span class="sxs-lookup"><span data-stu-id="b560b-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="b560b-114">Lisateavet leiate teemast [loomine SharePointi meeskonnasaidi](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="b560b-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

