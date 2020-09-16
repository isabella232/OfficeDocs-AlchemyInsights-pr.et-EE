---
title: Teave Yammeri identiteedi kohta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664166"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="12f74-102">Teave Yammeri identiteedi kohta</span><span class="sxs-lookup"><span data-stu-id="12f74-102">About identity in Yammer</span></span>

<span data-ttu-id="12f74-103">Identiteediga seotud probleemide vältimiseks soovitame kõigil võrkudel teha järgmisi toiminguid.</span><span class="sxs-lookup"><span data-stu-id="12f74-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="12f74-104">Office 365 identiteedi jõustamine pärast seda, kui Microsoft 365 on Azure AD kasutajatele ette valmistanud, veenduge, et kõik kasutajad logivad sisse oma peamise Microsoft 365 konto abil.</span><span class="sxs-lookup"><span data-stu-id="12f74-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="12f74-105">Lisateavet leiate teemast [Office 365 identiteedi jõustamine Yammeri kasutajate jaoks](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="12f74-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="12f74-106">Konsolideerida mitu Yammeri võrku.</span><span class="sxs-lookup"><span data-stu-id="12f74-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="12f74-107">Pärand Yammeri konfiguratsioonid võimaldavad mitu Yammeri võrku ühendada ühe rentniku jaoks.</span><span class="sxs-lookup"><span data-stu-id="12f74-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="12f74-108">Lisateavet leiate teemast [võrgu migreerimine – mitme Yammeri võrgu konsolideerimine](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="12f74-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="12f74-109">Soovi korral saate Yammeri kasutajatele blokeerida ka Yammeri litsentsimise, kui neil pole litsentsi.</span><span class="sxs-lookup"><span data-stu-id="12f74-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="12f74-110">Lisateavet leiate teemast [Yammeri kasutajate litsentside haldamine Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="12f74-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="12f74-111">Lõpetuseks auditeerige vanemate Yammeri võrkude kasutajate loendit ja katkestage pärandi kasutajad.</span><span class="sxs-lookup"><span data-stu-id="12f74-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="12f74-112">Soovitatav on kasutajate kustutamise asemel peatada (desaktiveerida), kuna kustutamine on pöördumatu.</span><span class="sxs-lookup"><span data-stu-id="12f74-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="12f74-113">Lisateavet leiate teemast [Yammeri kasutajate auditeerimine Office 365 ühendatud võrkudes](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) ja [kasutajate eemaldamine](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="12f74-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="12f74-114">Yammeri konfigureerimine nende juhiste abil saate ka oma Yammeri võrgu konfigureerida Microsoft 365-i emakeelena režiimis.</span><span class="sxs-lookup"><span data-stu-id="12f74-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="12f74-115">Lisateavet leiate teemast [Yammeri võrgu konfigureerimine Microsoft 365-i emakeelena režiimis](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="12f74-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>