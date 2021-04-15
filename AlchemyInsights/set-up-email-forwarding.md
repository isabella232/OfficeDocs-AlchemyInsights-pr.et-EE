---
title: Meili edasisaatmise häälestamine
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
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a7fba259375c667ff2e0f14a03972e102468cd27
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51787133"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="21132-102">Postkasti meili edasisaatmise sätete kontrollimine</span><span class="sxs-lookup"><span data-stu-id="21132-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="21132-103">Esiteks peab meilide edasisaatmine olema rentnikutasemel lubatud.</span><span class="sxs-lookup"><span data-stu-id="21132-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="21132-104">Kui olete häälestanud meilisõnumite edasisaatmise postkastis, kuid see ei tööta (kuvatakse tõrketeade **"550 5.7.520 Access denied, Your organization not allow external forwarding" ("550 5.7.520 Access denied, Your organization not allow external forwarding") ("550 5.7.520 Access denied, Your organization not allow external forwarding") ("550 5.7.520 Access denied, Your organization not allow external forwarding" (550 5.7.520 Access denied, Teie** asutus ei luba välist edasisaatmist) lugege teemat Automaatse välise meilisõnumite edasisaatmise juhtimine [Rakenduses Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="21132-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="21132-105">Meilisõnumite edasisaatmise sätete kontrollimine postkastis on lihtne!</span><span class="sxs-lookup"><span data-stu-id="21132-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="21132-106">Järgige neid juhiseid.</span><span class="sxs-lookup"><span data-stu-id="21132-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="21132-107">Kui see on kasutajapostkast,  avage Kasutajad Aktiivsed \> **kasutajad** ja valige kasutaja, kelle postkasti te edasi saadate.</span><span class="sxs-lookup"><span data-stu-id="21132-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="21132-108">Valige **vahekaardil Elektronpost** käsk **Halda meilisõnumite edasisaatmist**.</span><span class="sxs-lookup"><span data-stu-id="21132-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="21132-109">Kui see on ühispostkast, avage **Rühmad** \> **ühispostkastid** ja valige edasisaattav ühispostkast.</span><span class="sxs-lookup"><span data-stu-id="21132-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="21132-110">Meilisõnumite **edasisaatmiseks** valige Redigeeri.</span><span class="sxs-lookup"><span data-stu-id="21132-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="21132-111">Lisateavet leiate teemast [Meilisõnumite edasisaatmise konfigureerimine Microsoft 365-s.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="21132-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="21132-112">Kasutajatele juhiste saatmiseks, et nad saaksid häälestada meilisõnumite edasisaatmise oma postkastides, osutage neile väärtusele Meilisõnumite edasisaatmine [Microsoft 365-st teisele meilikontole.](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)</span><span class="sxs-lookup"><span data-stu-id="21132-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="21132-113">Võtke arvesse, et saate edasi saata ainult ühele meiliaadressile.</span><span class="sxs-lookup"><span data-stu-id="21132-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="21132-114">Kui peate häälestama edasisaatmise inimeste rühmale, looge leviloend (jaotises **Rühmad),** lisage sinna oma kasutajad ja konfigureerige edasisaatmine sellele rühmale.</span><span class="sxs-lookup"><span data-stu-id="21132-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="21132-115">Kas teil on töötaja lahkumas?</span><span class="sxs-lookup"><span data-stu-id="21132-115">Do you have an employee leaving?</span></span> <span data-ttu-id="21132-116">Soovitatavad [juhised leiate teemast Endise töötaja eemaldamine Microsoft 365-st.](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee)</span><span class="sxs-lookup"><span data-stu-id="21132-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>