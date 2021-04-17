---
title: Karantiinis puuduvad meilisõnumid
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831730"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="28d8d-102">Karantiinis puuduvad meilisõnumid"</span><span class="sxs-lookup"><span data-stu-id="28d8d-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="28d8d-103">Administraatorid saavad [neid sõnumeid vaadata, vabastada või kustutada.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="28d8d-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="28d8d-104">Turbe- & avamiseks avage [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="28d8d-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="28d8d-105">Karantiinilehe otse avamiseks avage [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="28d8d-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="28d8d-106">Saate otsida järgmiste väärtuste järgi.</span><span class="sxs-lookup"><span data-stu-id="28d8d-106">You can search by the following values:</span></span>  

- <span data-ttu-id="28d8d-107">**Sõnumi ID:** sõnumi globaalne ainuidentifikaator.</span><span class="sxs-lookup"><span data-stu-id="28d8d-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="28d8d-108">Kui valite loendist sõnumi, kuvatakse kuvataval hüpikpaanil **Üksikasjad** väärtus Sõnumi **ID.**</span><span class="sxs-lookup"><span data-stu-id="28d8d-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="28d8d-109">Administraatorid saavad [sõnumijälitus abil](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) otsida sõnumeid ja neile vastavaid sõnumi ID väärtusi.</span><span class="sxs-lookup"><span data-stu-id="28d8d-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="28d8d-110">**Saatja meiliaadress:** ühe saatja meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="28d8d-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="28d8d-111">**Adressaadi meiliaadress:** ühe adressaadi meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="28d8d-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="28d8d-112">**Teema:** kasutage kogu sõnumi teemat.</span><span class="sxs-lookup"><span data-stu-id="28d8d-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="28d8d-113">Otsing pole stiotsingutundlik.</span><span class="sxs-lookup"><span data-stu-id="28d8d-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="28d8d-114">Kui olete otsingukriteeriumid sisestanud, klõpsake ![ tulemite ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **filtreerimiseks** nuppu Värskenda.  </span><span class="sxs-lookup"><span data-stu-id="28d8d-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="28d8d-115">Cmdlet-käsud, mida kasutate sõnumite ja failide karantiinis kuvamiseks ja haldamiseks, on järgmised.</span><span class="sxs-lookup"><span data-stu-id="28d8d-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="28d8d-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="28d8d-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="28d8d-117">Ekspordi-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="28d8d-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="28d8d-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="28d8d-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="28d8d-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Pange tähele, et see cmdlet-käsk on ainult sõnumite, mitte ründevarafailide jaoks, mis on pärit SharePoint Online'i, OneDrive for Businessi või Teamsi ATP-st.</span><span class="sxs-lookup"><span data-stu-id="28d8d-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="28d8d-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="28d8d-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)