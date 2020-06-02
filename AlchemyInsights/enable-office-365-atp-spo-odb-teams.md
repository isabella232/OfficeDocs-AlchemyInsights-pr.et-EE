---
title: Office 365 ATP lubamine SharePointi, OneDrive ' i ja Microsofti meeskondade jaoks
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506914"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="49329-102">Lubage Office 365 täiustatud ohutõrje SharePoint Online ' i, OneDrive ja Microsoft Teamsi jaoks</span><span class="sxs-lookup"><span data-stu-id="49329-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="49329-103">https://protection.office.comsisse ja logige sisse.</span><span class="sxs-lookup"><span data-stu-id="49329-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="49329-104">Valige ohutaseme **halduse**  >  **poliitika**  >  **Turvalised manused**.</span><span class="sxs-lookup"><span data-stu-id="49329-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="49329-105">Valige **LÜLITA ATP SharePointi, OneDrive ja Microsoft Teams**ja seejärel klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="49329-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="49329-106">Soovitatav Globaalne administraator või SharePoint Online ' i administraator, käivitage cmdlet [-käsu Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) koos parameetri **Disallowinfectedfiledownload** väärtuseks *True*.</span><span class="sxs-lookup"><span data-stu-id="49329-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="49329-107">Soovitatav [Seadistage](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tuvastatud failide teatised.</span><span class="sxs-lookup"><span data-stu-id="49329-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="49329-108">ATP aitab skannida iga faili SharePoint Online, OneDrive või Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="49329-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="49329-109">Faile skannitakse asünkroonselt protsessi kaudu, mis kasutab ühiskasutuse ja külalistegevuste sündmusi koos nutikate heuristika ja ohusignaalidega, et tuvastada pahatahtlikke faile.</span><span class="sxs-lookup"><span data-stu-id="49329-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="49329-110">Vt [ATP SharePointi, OneDrive ' i ja Microsoft teamsi jaoks](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="49329-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>