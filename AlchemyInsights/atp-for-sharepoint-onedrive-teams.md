---
title: ATP SharePoint, OneDrive ja Microsoft meeskonnad
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764992"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="3e4df-102">ATP SharePoint, OneDrive ja Microsoft meeskonnad</span><span class="sxs-lookup"><span data-stu-id="3e4df-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="3e4df-103">Täiustatud ohutõrje lubamiseks tehke järgmist</span><span class="sxs-lookup"><span data-stu-id="3e4df-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="3e4df-104">Mine [https://protection.office.com](https://protection.office.com) ja logite sisse globaalne administraatori või turvalisuse administraatori konto.</span><span class="sxs-lookup"><span data-stu-id="3e4df-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="3e4df-105">Valige vasakpoolsel navigeerimispaanil alusel **ohu haldamise** **poliitika** \> **Safe Attachments**.</span><span class="sxs-lookup"><span data-stu-id="3e4df-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="3e4df-106">Valige **Lülita ATP SharePoint, OneDrive ja Microsoft meeskonnad**.</span><span class="sxs-lookup"><span data-stu-id="3e4df-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="3e4df-107">Saada teateid, kui tuvastame pahatahtlike faile [aktiivsus alert poliitika loomine](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) .</span><span class="sxs-lookup"><span data-stu-id="3e4df-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="3e4df-108">Täielike juhiste vaatamiseks vt see [teema](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="3e4df-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="3e4df-109">**Märkus**: Autor disain, ATP ei skanni iga ühe faili SharePoint Online, OneDrive äri-või Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3e4df-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="3e4df-110">Kontrollitakse faile asünkroonselt protsess, mis kasutab ühiskasutuse tegevuse, Külastajate tegevuse ja ohtu signaalide pahatahtlike faile tuvastada.</span><span class="sxs-lookup"><span data-stu-id="3e4df-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="3e4df-111">Lisateavet vt selle [teema](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="3e4df-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>