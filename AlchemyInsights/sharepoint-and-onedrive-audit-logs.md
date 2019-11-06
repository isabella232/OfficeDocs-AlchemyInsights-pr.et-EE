---
title: Klassikaline SharePointi auditilogi aruanded
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992614"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="882fb-102">SharePointi ja OneDrive ' i auditilogi</span><span class="sxs-lookup"><span data-stu-id="882fb-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="882fb-103">SharePointi klassikaline auditilogi</span><span class="sxs-lookup"><span data-stu-id="882fb-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="882fb-104">SPO pärand auditeerimine migreeritakse Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="882fb-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="882fb-105">Kõik SPO pärand auditi aruanded on nüüd powered by UAL ja pärand auditi signaale on migreeritud UAL.</span><span class="sxs-lookup"><span data-stu-id="882fb-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="882fb-106">Peamised muudatused:</span><span class="sxs-lookup"><span data-stu-id="882fb-106">Key changes:</span></span>

* <span data-ttu-id="882fb-107">Korrastamine ei ole võimetena saadaval.</span><span class="sxs-lookup"><span data-stu-id="882fb-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="882fb-108">Konkreetsete sündmuste valimine auditiga pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="882fb-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="882fb-109">Vaadake [seda dokumenti](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) vaikimisi saadaolevate auditeeritud sündmuste täieliku loendi kohta.</span><span class="sxs-lookup"><span data-stu-id="882fb-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="882fb-110">**Kohandatud aruannete** all **asukoht** suvand pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="882fb-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="882fb-111">**Dokumentide avamine või allalaadimine** suvand sündmused pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="882fb-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="882fb-112">Saidikogumi Auditisätete konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="882fb-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="882fb-113">SharePointi ja OneDrive kaasaegne ühendatud audit logib vastavuse</span><span class="sxs-lookup"><span data-stu-id="882fb-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="882fb-114">Lülita sisse/välja ühendatud auditilogi logimine</span><span class="sxs-lookup"><span data-stu-id="882fb-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="882fb-115">SharePoint või OneDrive ei vaja täiendavat konfiguratsiooni.</span><span class="sxs-lookup"><span data-stu-id="882fb-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="882fb-116">Auditilogi otsingu abil saate kontrollida faili (de), kausta (de), kasutaja (te), õigusi:</span><span class="sxs-lookup"><span data-stu-id="882fb-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="882fb-117">Faili-ja lehetegevused</span><span class="sxs-lookup"><span data-stu-id="882fb-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="882fb-118">Kausta tegevused</span><span class="sxs-lookup"><span data-stu-id="882fb-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="882fb-119">Jagamise ja juurdepääsu taotluse tegevused</span><span class="sxs-lookup"><span data-stu-id="882fb-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="882fb-120">Sünkroonimise tegevused</span><span class="sxs-lookup"><span data-stu-id="882fb-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="882fb-121">Saidihalduse tegevused</span><span class="sxs-lookup"><span data-stu-id="882fb-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="882fb-122">Lisateavet nende sündmuste kohta leiate teemast [auditilogi otsing](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="882fb-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
