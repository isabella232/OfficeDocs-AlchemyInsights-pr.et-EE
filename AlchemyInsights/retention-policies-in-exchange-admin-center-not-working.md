---
title: Exchange'i halduskeskuse säilituspoliitikad ei tööta
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952224"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="bf392-102">Säilituspoliitikad Exchange'i halduskeskuses</span><span class="sxs-lookup"><span data-stu-id="bf392-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="bf392-103">Kui soovite, et käivitame allpool nimetatud sätete automaatsed kontrollid, valige selle lehe ülaservas nupp < ja sisestage säilituspoliitikatega seotud probleemidega kasutaja meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="bf392-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="bf392-104">Kui teil on Exchange'i halduskeskuse säilituspoliitikatega probleeme, mis ei kehti postkastidele või üksustele, mis ei teisalda arhiivipostkasti, kontrollige järgmist.</span><span class="sxs-lookup"><span data-stu-id="bf392-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="bf392-105">**Juurpõhjused:**</span><span class="sxs-lookup"><span data-stu-id="bf392-105">**Root Causes:**</span></span>

- <span data-ttu-id="bf392-106">**Hallatud** kaustaabimees ei ole kasutaja postkasti töötlenud.</span><span class="sxs-lookup"><span data-stu-id="bf392-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="bf392-107">Hallatava kausta abiline proovib töödelda iga postkasti teie pilvepõhises organisatsioonis üks kord seitsme päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="bf392-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="bf392-108">**Lahendus:** Käivitage hallatud kaustaabimees.</span><span class="sxs-lookup"><span data-stu-id="bf392-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="bf392-109">**Säilituspeetus** on **postkastis** lubatud.</span><span class="sxs-lookup"><span data-stu-id="bf392-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="bf392-110">Kui postkast on paigutatud säilitusapeetusse, siis selle aja jooksul postkasti säilituspoliitikat ei töödelda.</span><span class="sxs-lookup"><span data-stu-id="bf392-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="bf392-111">**Lahendus:** Kontrollige säilitussätte olekut ja värskendage seda vastavalt vajadusele.</span><span class="sxs-lookup"><span data-stu-id="bf392-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="bf392-112">Lisateavet leiate teemast [Postkasti säilituse ootel hoidmine.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="bf392-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="bf392-113">**Märkus.** Kui postkast on väiksem kui 10 MB, ei töötle hallatava kausta abiline postkasti automaatselt.</span><span class="sxs-lookup"><span data-stu-id="bf392-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="bf392-114">Lisateavet Säilituspoliitikate kohta Exchange'i halduskeskuses leiate järgmisest teemast.</span><span class="sxs-lookup"><span data-stu-id="bf392-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="bf392-115">Säilitussildid ja säilituspoliitikad</span><span class="sxs-lookup"><span data-stu-id="bf392-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="bf392-116">[Säilituspoliitika rakendumine postkastidele või](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [säilitussiltide lisamine või eemaldamine](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="bf392-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="bf392-117">Postkasti paigutatud ootel salvestatud ootele pandud tüübi tuvastamine</span><span class="sxs-lookup"><span data-stu-id="bf392-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
