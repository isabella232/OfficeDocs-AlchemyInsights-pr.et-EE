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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801043"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="eb08d-102">Microsoft Defenderi Office 365 for SharePoint Online ' i, OneDrive ' i ja Microsoft Teamsi jaoks lubamine</span><span class="sxs-lookup"><span data-stu-id="eb08d-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="eb08d-103">Avage https://protection.office.com ja logige sisse.</span><span class="sxs-lookup"><span data-stu-id="eb08d-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="eb08d-104">Valige **ohustatud halduse**  >  **poliitika**  >  **Turvalised manused** .</span><span class="sxs-lookup"><span data-stu-id="eb08d-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="eb08d-105">Valige **Lülita SharePointi, OneDrive ' i ja Microsoft teamsi jaoks ATP** ja seejärel klõpsake nuppu **Salvesta** .</span><span class="sxs-lookup"><span data-stu-id="eb08d-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="eb08d-106">Soovitatav Globaalse administraatorina või SharePoint Online ' i administraatorina käivitage cmdlet [-käsk Set-spotenantiga](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) , mille parameeter **DisallowInfectedFileDownload** on seatud väärtusele *True* .</span><span class="sxs-lookup"><span data-stu-id="eb08d-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="eb08d-107">Soovitatav [Häälestage](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tuvastatud failide teatised.</span><span class="sxs-lookup"><span data-stu-id="eb08d-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="eb08d-108">ATP saab nSeadete skannida kõik failid SharePoint Online ' is, OneDrive ' is või Microsoft Teamsi.</span><span class="sxs-lookup"><span data-stu-id="eb08d-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="eb08d-109">Failid skannitakse asünkroonselt kaudu, mis kasutab ühiskasutust ja Guest Activity üritusi, ning nutikad heuristilined ja ohud, et tuvastada pahatahtlikud failid.</span><span class="sxs-lookup"><span data-stu-id="eb08d-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="eb08d-110">Lugege teemat [SharePointi, OneDrive ' i ja Microsoft teamsi ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="eb08d-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>