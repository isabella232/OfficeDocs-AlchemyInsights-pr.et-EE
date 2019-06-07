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
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758727"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="d4c69-102">Luua rühma ühendatud saidi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d4c69-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="d4c69-103">On ühiseid teemasid kui ühendatud loomine või uuesti luua rühma saidi paar.</span><span class="sxs-lookup"><span data-stu-id="d4c69-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="d4c69-104">Kui rühma ja sellega seotud saidi kustutanud ja soovite luua teisele saidile sama URL-iga, peate eelmisest jäädavalt eemaldada.</span><span class="sxs-lookup"><span data-stu-id="d4c69-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="d4c69-105">Lae [SPO halduskestas](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="d4c69-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="d4c69-106">Rohkem infot kuidas alustada PowerShelli abil, vaadake [SharePoint Online halduskesta alustamine](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="d4c69-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="d4c69-107">Eemalda saidi kustutada saidid kasutades [Eemalda-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShelli cmdlet-i.</span><span class="sxs-lookup"><span data-stu-id="d4c69-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="d4c69-108">Kui rühma ühendatud saidi loomisel kuvatakse hoiatus, teine rühm sama pseudonüüm on juba olemas, kontrollige [Office 365 halduskeskuse kaudu](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)olemasolevatesse gruppidesse.</span><span class="sxs-lookup"><span data-stu-id="d4c69-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="d4c69-109">Probleemi lahendamiseks, olemasoleva rühma kustutada, kui see ei ole enam vajalik või luua saidi eri alias määratud.</span><span class="sxs-lookup"><span data-stu-id="d4c69-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="d4c69-110">On erinevaid viise, kuidas luua ja kasutada kaasaegseid sõprade SharePointiga.</span><span class="sxs-lookup"><span data-stu-id="d4c69-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="d4c69-111">Interneti Office 365 rühma olemasolevatel saitidel.</span><span class="sxs-lookup"><span data-stu-id="d4c69-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="d4c69-112">Lisateavet leiate teemast [ühendamine Office 365 rühma, kasutades SharePointi kasutaja ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="d4c69-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="d4c69-113">Office 365 rühma ühendatud saidi loomiseks peate luua meeskonnatöö veebisaidi.</span><span class="sxs-lookup"><span data-stu-id="d4c69-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="d4c69-114">Lisateavet leiate teemast [loomine SharePointi meeskonnasaidi](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="d4c69-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

