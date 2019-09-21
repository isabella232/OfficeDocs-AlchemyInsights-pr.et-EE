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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068019"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="2070a-102">SharePointi ja OneDrive ' i auditilogi</span><span class="sxs-lookup"><span data-stu-id="2070a-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="2070a-103">**SharePointi ja OneDrive kaasaegne ühendatud audit logib vastavuse**</span><span class="sxs-lookup"><span data-stu-id="2070a-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="2070a-104">Lülita sisse/välja ühendatud auditilogi logimine</span><span class="sxs-lookup"><span data-stu-id="2070a-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="2070a-105">SharePoint või OneDrive ei vaja täiendavat konfiguratsiooni.</span><span class="sxs-lookup"><span data-stu-id="2070a-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="2070a-106">Auditilogi otsingu abil saate kontrollida faili (de), kausta (de), kasutaja (te), õigusi:</span><span class="sxs-lookup"><span data-stu-id="2070a-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="2070a-107">Faili-ja lehetegevused</span><span class="sxs-lookup"><span data-stu-id="2070a-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="2070a-108">Kausta tegevused</span><span class="sxs-lookup"><span data-stu-id="2070a-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="2070a-109">Jagamise ja juurdepääsu taotluse tegevused</span><span class="sxs-lookup"><span data-stu-id="2070a-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="2070a-110">Sünkroonimise tegevused</span><span class="sxs-lookup"><span data-stu-id="2070a-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="2070a-111">Saidihalduse tegevused</span><span class="sxs-lookup"><span data-stu-id="2070a-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="2070a-112">Lisateavet nende sündmuste kohta leiate teemast [auditilogi otsing](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="2070a-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="2070a-113">**SharePointi klassikaline auditilogi**</span><span class="sxs-lookup"><span data-stu-id="2070a-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="2070a-114">Me migreerisime SPO pärand auditeerimine Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="2070a-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="2070a-115">See tähendab sisuliselt, et kõik SPO pärand auditiaruanded on nüüd läbi UAL ja pärand auditi signaale on migreeritud UAL.</span><span class="sxs-lookup"><span data-stu-id="2070a-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="2070a-116">Peamised muudatused:</span><span class="sxs-lookup"><span data-stu-id="2070a-116">Key changes:</span></span>

- <span data-ttu-id="2070a-117">Korrastamine võimetena ei ole saadaval.</span><span class="sxs-lookup"><span data-stu-id="2070a-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="2070a-118">Jaotis, kus saate auditeerimiseks konkreetseid sündmusi valida, pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="2070a-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="2070a-119">Palun vaadake [seda dokumenti](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) vaikimisi saadaolevate auditeeritud sündmuste täieliku loendi kohta.</span><span class="sxs-lookup"><span data-stu-id="2070a-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="2070a-120">**Kohandatud aruannete** all suvand "asukoht" pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="2070a-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="2070a-121">"Dokumentide avamine või allalaadimine" sündmused pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="2070a-121">“Opening or downloading documents” events is NOT available.</span></span> 

