---
title: Auditeerimine rakenduses Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429645"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="fffa6-102">Auditeerimine rakenduses Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fffa6-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="fffa6-103">Siin on mõned asjad, mida peaksite Microsoft 365 auditeerimise kohta teadma.</span><span class="sxs-lookup"><span data-stu-id="fffa6-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="fffa6-104">Exchange ' i administraatori tegevusi auditeeritakse vaikimisi.</span><span class="sxs-lookup"><span data-stu-id="fffa6-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="fffa6-105">Oleme postkasti auditeerimise käigus kõigi kasutajate jaoks vaikimisi sisse lülitanud.</span><span class="sxs-lookup"><span data-stu-id="fffa6-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="fffa6-106">Selle kohta lisateabe saamiseks klõpsake [siin](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span><span class="sxs-lookup"><span data-stu-id="fffa6-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="fffa6-107">Kuni selle ajani, kui soovite juhiseid selle isiku või kogu asutuse käsitsi lubamiseks, valige allpool nupp Lülita postkasti audit.</span><span class="sxs-lookup"><span data-stu-id="fffa6-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="fffa6-108">Microsoft 365 rühmade postkastid ja ühiskausta postkastid ei toeta auditi logimist.</span><span class="sxs-lookup"><span data-stu-id="fffa6-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="fffa6-109">SharePointi/OneDrive ' i jaoks pole auditeerimise lubamiseks vaja täiendavaid konfiguratsioone.</span><span class="sxs-lookup"><span data-stu-id="fffa6-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="fffa6-110">Tegevuste auditeerimise kohta leiate teavet järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="fffa6-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="fffa6-111">Pilt tegevused</span><span class="sxs-lookup"><span data-stu-id="fffa6-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="fffa6-112">Kausta tegevused</span><span class="sxs-lookup"><span data-stu-id="fffa6-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="fffa6-113">[Ühiskasutus ja juurdepääs tegevustele](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span><span class="sxs-lookup"><span data-stu-id="fffa6-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="fffa6-114">Kõigi auditeeritud tegevuste loendi leiate teemast [auditeeritud tegevused](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="fffa6-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
