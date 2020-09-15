---
title: ATP SharePointi, OneDrive ' i ja Microsoft Teamsi jaoks
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715557"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="da4f3-102">ATP SharePointi, OneDrive ' i ja Microsoft Teamsi jaoks</span><span class="sxs-lookup"><span data-stu-id="da4f3-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="da4f3-103">Täpsema ohu kaitse lubamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="da4f3-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="da4f3-104">Avage [https://protection.office.com](https://protection.office.com) ja logige sisse üldise administraatori või administraatori kontoga.</span><span class="sxs-lookup"><span data-stu-id="da4f3-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="da4f3-105">Valige vasakpoolsel navigeerimispaanil jaotises **ohu haldamine**suvand **poliitika** \> **ohutud manused**.</span><span class="sxs-lookup"><span data-stu-id="da4f3-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="da4f3-106">Valige suvand **Lülita SharePointi, OneDrive ' i ja Microsoft teamsi jaoks välja ATP**.</span><span class="sxs-lookup"><span data-stu-id="da4f3-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="da4f3-107">[Saate luua tegevuse teatise poliitika](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) , et saada teatisi, kui oleme tuvastanud pahatahtlikud failid.</span><span class="sxs-lookup"><span data-stu-id="da4f3-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="da4f3-108">Juhised leiate [teemast](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="da4f3-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="da4f3-109">**Märkus**: kujunduse järgi ei kontrolli ATP kõiki SharePoint Online ' i, OneDrive for Businessi või Microsoft teamsi faile.</span><span class="sxs-lookup"><span data-stu-id="da4f3-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="da4f3-110">Faile skannitakse asünkroonselt abil, mis kasutab pahatahtlike failide tuvastamiseks ühiskasutuse tegevust, Külastajate tegevust ja ähvardavaid signaale.</span><span class="sxs-lookup"><span data-stu-id="da4f3-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="da4f3-111">Lisateavet leiate sellest [teemast](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="da4f3-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
