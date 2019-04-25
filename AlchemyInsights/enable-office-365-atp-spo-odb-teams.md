---
title: Office 365 ATP lubamine SharePoint, OneDrive ja Microsoft meeskonnad
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403029"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1f0fb-102">Luba Office 365 arenenud oht kaitse SharePoint Online, OneDrive ja Microsoft meeskonnad</span><span class="sxs-lookup"><span data-stu-id="1f0fb-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="1f0fb-103">Mine https://protection.office.com ja logige sisse.</span><span class="sxs-lookup"><span data-stu-id="1f0fb-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="1f0fb-104">Valida **ohu haldamise** > **poliitika** > **Safe Attachments**.</span><span class="sxs-lookup"><span data-stu-id="1f0fb-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="1f0fb-105">Valige **ATP SharePoint, OneDrive ja Microsoft meeskonnad sisse lülitada**ja klõpsake siis nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="1f0fb-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="1f0fb-106">(Soovitatav) Globaalne administraatori või SharePoint Online'i administraatori, käivitada [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet-käsu parameetri **DisallowInfectedFileDownload** väärtuseks *tõene*.</span><span class="sxs-lookup"><span data-stu-id="1f0fb-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="1f0fb-107">(Soovitatav) Tuvastatud failide [hoiatuste häälestus](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) .</span><span class="sxs-lookup"><span data-stu-id="1f0fb-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="1f0fb-108">ATP on nto skaneerida iga ühe faili SharePoint Online, OneDrive või Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1f0fb-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="1f0fb-109">Asünkroonselt, kontrollitakse läbi protsessi, mis kasutab jagamine ja Külastajate tegevuse võistlusi, koos smart heuristics ja ohtu signaale pahatahtlike faile tuvastada faile.</span><span class="sxs-lookup"><span data-stu-id="1f0fb-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="1f0fb-110">Vaadake [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="1f0fb-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>