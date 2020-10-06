---
title: Meilisõnumite kohaletoimetamisega seotud probleemide lahendamine meililoaga ühiskaustade korral
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
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366460"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="b8f3d-102">Meilisõnumite kohaletoimetamisega seotud probleemide lahendamine meililoaga ühiskaustade korral</span><span class="sxs-lookup"><span data-stu-id="b8f3d-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="b8f3d-103">Kui välised saatjad ei saa saata meilisõnumeid teie meililoaga ühiskaustu ja saatjad saavad tõrketeate: **ei leita (550 5.4.1)**, veenduge, et ühiskausta Domeen oleks konfigureeritud autoriteetse domeeni asemel asutusesiseseks edastamise domeeniks.</span><span class="sxs-lookup"><span data-stu-id="b8f3d-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="b8f3d-104">Avage [Exchange ' i halduskeskus (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="b8f3d-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="b8f3d-105">Avage jaotis **meilivoo** \> **aktsepteeritud domeenid**, valige aktsepteeritud domeen ja klõpsake nuppu **Redigeeri**.</span><span class="sxs-lookup"><span data-stu-id="b8f3d-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="b8f3d-106">Kui domeeni tüüp on seatud **autoriteetseks**, muutke kuvatavas atribuutide lehel väärtust **sisemine edastus** ja seejärel klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="b8f3d-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="b8f3d-107">Kui välised saatjad saavad tõrketeate **(550 5.7.13)**, käivitage [Exchange Online PowerShellis](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) järgmine käsk, et kuvada anonüümsete kasutajate õigused avalikus kaustas.</span><span class="sxs-lookup"><span data-stu-id="b8f3d-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="b8f3d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Näiteks `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="b8f3d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="b8f3d-109">Kui soovite, et väliskasutajad saaksid selle ühiskausta meilisõnumeid saata, lisage CreateItems juurdepääs otse kasutajale anonüümseks.</span><span class="sxs-lookup"><span data-stu-id="b8f3d-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="b8f3d-110">Näiteks `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="b8f3d-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
