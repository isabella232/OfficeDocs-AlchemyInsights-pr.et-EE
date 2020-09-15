---
title: Office 365 ATP lubamine SharePointi, OneDrive ' i ja Microsoft Teamsi jaoks
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709903"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="57362-102">SharePoint Online ' i, OneDrive ' i ja Microsoft Teamsi jaoks mõeldud Office 365 täiustatud ohu kaitse lubamine</span><span class="sxs-lookup"><span data-stu-id="57362-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="57362-103">Avage https://protection.office.com ja logige sisse.</span><span class="sxs-lookup"><span data-stu-id="57362-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="57362-104">Valige **ohustatud halduse**  >  **poliitika**  >  **Turvalised manused**.</span><span class="sxs-lookup"><span data-stu-id="57362-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="57362-105">Valige **Lülita SharePointi, OneDrive ' i ja Microsoft teamsi jaoks ATP**ja seejärel klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="57362-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="57362-106">Soovitatav Globaalse administraatorina või SharePoint Online ' i administraatorina käivitage cmdlet [-käsk Set-spotenantiga](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) , mille parameeter **DisallowInfectedFileDownload** on seatud väärtusele *True*.</span><span class="sxs-lookup"><span data-stu-id="57362-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="57362-107">Soovitatav [Häälestage](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tuvastatud failide teatised.</span><span class="sxs-lookup"><span data-stu-id="57362-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="57362-108">ATP saab nSeadete skannida kõik failid SharePoint Online ' is, OneDrive ' is või Microsoft Teamsi.</span><span class="sxs-lookup"><span data-stu-id="57362-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="57362-109">Failid skannitakse asünkroonselt kaudu, mis kasutab ühiskasutust ja Guest Activity üritusi, ning nutikad heuristilined ja ohud, et tuvastada pahatahtlikud failid.</span><span class="sxs-lookup"><span data-stu-id="57362-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="57362-110">Lugege teemat [SharePointi, OneDrive ' i ja Microsoft teamsi ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="57362-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>