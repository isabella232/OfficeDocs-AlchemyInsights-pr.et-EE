---
title: Klassikalised SharePointi auditilogi aruanded
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662204"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="69588-102">SharePointi ja OneDrive ' i auditi logid</span><span class="sxs-lookup"><span data-stu-id="69588-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="69588-103">SharePointi klassikalise auditi logid</span><span class="sxs-lookup"><span data-stu-id="69588-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="69588-104">SPO Legacy audit viidi üle ühtsele auditi logile (UAL).</span><span class="sxs-lookup"><span data-stu-id="69588-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="69588-105">Kõik SPO pärandi auditi aruanded on nüüd powered kaudu UAL ja pärandi auditi signaalid on migreeritud UAL.</span><span class="sxs-lookup"><span data-stu-id="69588-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="69588-106">Olulisemad muudatused.</span><span class="sxs-lookup"><span data-stu-id="69588-106">Key changes:</span></span>

* <span data-ttu-id="69588-107">Kärpimine pole võimete jaoks saadaval.</span><span class="sxs-lookup"><span data-stu-id="69588-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="69588-108">Kindlate sündmuste valimine auditeerimiseks pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="69588-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="69588-109">Vaikimisi saadaolevate auditeeritud sündmuste loendi leiate [sellest dokumendist](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) .</span><span class="sxs-lookup"><span data-stu-id="69588-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="69588-110">Suvand **asukoht** **kohandatud aruannetes** pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="69588-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="69588-111">Suvand **dokumentide avamine või allalaadimine** pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="69588-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="69588-112">Saidikogumi auditi sätete konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="69588-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="69588-113">SharePointi ja OneDrive ' i kaasaegsed ühtsed auditi logid vastavusest</span><span class="sxs-lookup"><span data-stu-id="69588-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="69588-114">Unified auditilogi sisse-/väljalülitamine</span><span class="sxs-lookup"><span data-stu-id="69588-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="69588-115">SharePointis või OneDrive ' is ei nõuta täiendavaid konfiguratsioone.</span><span class="sxs-lookup"><span data-stu-id="69588-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="69588-116">Auditi logimise otsingu abil saate kontrollida, kas failid (ID), kaustad (ID), kasutaja (d), permissions:</span><span class="sxs-lookup"><span data-stu-id="69588-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="69588-117">Failid ja lehe tegevused</span><span class="sxs-lookup"><span data-stu-id="69588-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="69588-118">Kausta tegevused</span><span class="sxs-lookup"><span data-stu-id="69588-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="69588-119">Ühiskasutuse ja juurdepääsu taotlemise toimingud</span><span class="sxs-lookup"><span data-stu-id="69588-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="69588-120">Sünkroonimise tegevused</span><span class="sxs-lookup"><span data-stu-id="69588-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="69588-121">Saidi halduse tegevused</span><span class="sxs-lookup"><span data-stu-id="69588-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="69588-122">Lisateavet nende sündmuste toomise kohta leiate teemast [auditilogi otsimine](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="69588-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
