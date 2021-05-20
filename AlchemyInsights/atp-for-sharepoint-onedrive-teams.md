---
title: Microsoft Defender Office 365 jaoks SharePoint, OneDrive ja Microsoft Teams
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
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543573"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="def86-102">Microsoft Defender Office 365 jaoks SharePoint, OneDrive ja Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="def86-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="def86-103">Microsoft Defender for Office 365 lubamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="def86-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="def86-104">Avage [https://protection.office.com](https://protection.office.com) üldadministraatori või turbeadministraatori konto ja logige sisse.</span><span class="sxs-lookup"><span data-stu-id="def86-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="def86-105">Klõpsake vasakpoolsel navigeerimispaanil **jaotises Ohuhaldus** nuppu **Poliitika** \> **ja seif Manused**.</span><span class="sxs-lookup"><span data-stu-id="def86-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="def86-106">Valige **Lülita Office 365 jaoks SharePoint, OneDrive ja Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="def86-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="def86-107">[Looge tegevusteatise poliitika,](/microsoft-365/compliance/create-activity-alerts) et saada teatisi, kui tuvastame pahatahtlikke faile.</span><span class="sxs-lookup"><span data-stu-id="def86-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="def86-108">Täielikud juhised leiate teemast [Seif, SharePoint, OneDrive ja Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="def86-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="def86-109">**Märkus.** Microsoft Defender Office 365 ei skanni SharePoint Online'is, OneDrive for Business või Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="def86-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="def86-110">Faile kontrollib asünkroonselt protsess, mis kasutab pahatahtlike failide tuvastamiseks ühiskasutustegevust, külalistegevust ja ohusignaale.</span><span class="sxs-lookup"><span data-stu-id="def86-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="def86-111">Lisateavet leiate teemast [seif Manused SharePoint, OneDrive ja Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="def86-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
