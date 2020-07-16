---
title: Teave identiteedi kohta Yammeris
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148235"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="30597-102">Teave identiteedi kohta Yammeris</span><span class="sxs-lookup"><span data-stu-id="30597-102">About identity in Yammer</span></span>

<span data-ttu-id="30597-103">Identiteediga seotud probleemide vältimiseks on soovitatav, et kõik võrgud võtaksid järgmist.</span><span class="sxs-lookup"><span data-stu-id="30597-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="30597-104">Jõustada Office 365 identiteedi pärast ettevalmistamine Microsoft 365 kontode kasutajatele Azure AD veendumaks, et kõik kasutajad sisse logida, kasutades oma esmane Microsoft 365 konto.</span><span class="sxs-lookup"><span data-stu-id="30597-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="30597-105">Lisateavet leiate teemast [Office 365 identiteedi jõustamine Yammeri kasutajate jaoks](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="30597-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="30597-106">Konsolideerige mitu Yammeri võrku.</span><span class="sxs-lookup"><span data-stu-id="30597-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="30597-107">Pärand Yammeri konfiguratsioonid võimaldavad mitme Yammeri võrgu ühe rentnikuga ühendada.</span><span class="sxs-lookup"><span data-stu-id="30597-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="30597-108">Lisateavet leiate teemast [Võrgu migreerimine – mitme Yammeri võrgu konsolideerimine](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="30597-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="30597-109">Soovi korral jõustage Yammeri litsentsimine, et blokeerida kasutajad Yammerist, kui neil pole litsentsi.</span><span class="sxs-lookup"><span data-stu-id="30597-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="30597-110">Lisateavet leiate teemast [Yammeri kasutajalitsentside haldamine teenusekomplektis Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="30597-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="30597-111">Lõpuks auditeerida kasutajate loend vanemate Yammeri võrkude ja peatada pärand kasutajad.</span><span class="sxs-lookup"><span data-stu-id="30597-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="30597-112">Soovitatav on kasutajad kustutamise asemel peatada (desaktiveerida) kuna kustutamine on pöördumatu.</span><span class="sxs-lookup"><span data-stu-id="30597-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="30597-113">Lisateavet leiate teemast [Yammeri kasutajate auditeerimine teenusekomplektiga Office 365 ühendatud võrkudes](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) ja [Kasutajate eemaldamine](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="30597-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="30597-114">Yammeri konfigureerimisel nende juhiste abil saate konfigureerida ka oma Yammeri võrgu Microsoft 365 native mode jaoks.</span><span class="sxs-lookup"><span data-stu-id="30597-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="30597-115">Lisateavet leiate teemast [Yammeri võrgu konfigureerimine Microsoft 365 native mode jaoks](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="30597-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>