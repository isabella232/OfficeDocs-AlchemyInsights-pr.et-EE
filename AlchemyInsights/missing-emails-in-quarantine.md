---
title: Karantiinis puuduvad e-kirjad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569048"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="6100e-102">Karantiinis puuduvad meilid "</span><span class="sxs-lookup"><span data-stu-id="6100e-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="6100e-103">Administraatorid saavad [neid sõnumeid vaadata, vabastada või kustutada.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="6100e-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="6100e-104">Turvalisuse & vastavuse keskuse avamiseks [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="6100e-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="6100e-105">Otse karantiini lehe avamiseks [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="6100e-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="6100e-106">Saate otsida järgmiste väärtuste järgi:</span><span class="sxs-lookup"><span data-stu-id="6100e-106">You can search by the following values:</span></span>  

- <span data-ttu-id="6100e-107">**Sõnumi ID**: globaalne kordumatu identifikaator.</span><span class="sxs-lookup"><span data-stu-id="6100e-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="6100e-108">Kui valite loendist sõnumi, kuvatakse kuvatava **üksikasjade** hüpik- **sõnumi ID** väärtus.</span><span class="sxs-lookup"><span data-stu-id="6100e-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="6100e-109">Administraatorid saavad kasutada [sõnumi jälg](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) leida sõnumeid ja nende vastava sõnumi ID väärtused.</span><span class="sxs-lookup"><span data-stu-id="6100e-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="6100e-110">**Saatja e-posti aadress**: ühe saatja meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="6100e-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="6100e-111">**Adressaadi e-posti aadress**: ühe adressaadi meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="6100e-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="6100e-112">**Teema**: kasutage sõnumi tervet teemat.</span><span class="sxs-lookup"><span data-stu-id="6100e-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="6100e-113">Otsing ei ole tõstutundlik.</span><span class="sxs-lookup"><span data-stu-id="6100e-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="6100e-114">Pärast otsingukriteeriumide sisestamist klõpsake tulemuste filtreerimiseks nuppu Värskenda ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** .  </span><span class="sxs-lookup"><span data-stu-id="6100e-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="6100e-115">Cmdlet-käsud abil saate vaadata ja hallata karantiini sõnumeid ja faile on:</span><span class="sxs-lookup"><span data-stu-id="6100e-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="6100e-116">Kustuta-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="6100e-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="6100e-117">Eksport-Kvarantinemessage</span><span class="sxs-lookup"><span data-stu-id="6100e-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="6100e-118">Hankige-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="6100e-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="6100e-119">[Eelvaade-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): pange tähele, et see cmdlet-käsk on ainult sõnumeid, mitte PAHAVARA faile ATP SharePoint Online, OneDrive for Business või meeskonnad.</span><span class="sxs-lookup"><span data-stu-id="6100e-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="6100e-120">Vabastamine-Kvarantinemessage</span><span class="sxs-lookup"><span data-stu-id="6100e-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)