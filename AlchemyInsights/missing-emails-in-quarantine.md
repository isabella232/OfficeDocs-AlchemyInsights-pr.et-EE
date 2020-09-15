---
title: Puuduvad meilid karantiinis
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673710"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="7950f-102">Puuduvad meilid karantiinis "</span><span class="sxs-lookup"><span data-stu-id="7950f-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="7950f-103">Administraatorid saavad [neid sõnumeid vaadata, vabastada või kustutada.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="7950f-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="7950f-104">Turbe & täitmise keskuse avamiseks valige [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="7950f-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="7950f-105">Otse karantiini lehe avamiseks avage [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="7950f-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="7950f-106">Saate otsida järgmiste väärtuste järgi.</span><span class="sxs-lookup"><span data-stu-id="7950f-106">You can search by the following values:</span></span>  

- <span data-ttu-id="7950f-107">**Sõnumi ID**: sõnumi globaalselt kordumatu identifikaator.</span><span class="sxs-lookup"><span data-stu-id="7950f-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="7950f-108">Kui valite loendist sõnumi, kuvatakse kuvatavas hüpik paanil **sõnumi ID** väärtus. **Details**</span><span class="sxs-lookup"><span data-stu-id="7950f-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="7950f-109">Administraatorid saavad sõnumite otsimiseks ja vastavate sõnumi ID-väärtuste otsimiseks kasutada [sõnumi jälgi](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) .</span><span class="sxs-lookup"><span data-stu-id="7950f-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="7950f-110">**Saatja**meiliaadress: ühe saatja meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="7950f-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="7950f-111">**Adressaadi meiliaadress**: ühe adressaadi meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="7950f-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="7950f-112">**Teema**: kasutage sõnumi kogu teemat.</span><span class="sxs-lookup"><span data-stu-id="7950f-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="7950f-113">Otsing pole tõstutundlik.</span><span class="sxs-lookup"><span data-stu-id="7950f-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="7950f-114">Kui olete otsingukriteeriumid sisestanud, klõpsake ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** tulemite filtreerimiseks nuppu Värskenda.  </span><span class="sxs-lookup"><span data-stu-id="7950f-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="7950f-115">Karantiinis olevate sõnumite ja failide vaatamiseks ja haldamiseks kasutatavad cmdlet-käsud on järgmised.</span><span class="sxs-lookup"><span data-stu-id="7950f-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="7950f-116">Kustutamine – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="7950f-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="7950f-117">Eksport – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="7950f-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="7950f-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="7950f-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="7950f-119">[Eelvaade – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): pange tähele, et see cmdlet on mõeldud ainult sõnumitele, mitte ründevarale SharePoint Online ' i, OneDrive for Businessi või TEAMsi ATP-St.</span><span class="sxs-lookup"><span data-stu-id="7950f-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="7950f-120">Väljalase – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="7950f-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)