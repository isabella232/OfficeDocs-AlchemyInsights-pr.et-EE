---
title: E-posti kohaletoimetamise lahendamine meililoaga Ühiskaustad
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910591"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="6dad9-102">E-posti kohaletoimetamise lahendamine meililoaga Ühiskaustad</span><span class="sxs-lookup"><span data-stu-id="6dad9-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="6dad9-103">Kui välistelt saatjatelt ei saa sõnumeid saata meililoaga avalike kaustade ja nende saatjad saavad viga: **ei suutnud leida (550 5.4.1)**, kontrollige e-posti domeeni jaoks ühiskaust on konfigureeritud sisemiseks vahedomeeniks asemel on autoriteetne Domeen:</span><span class="sxs-lookup"><span data-stu-id="6dad9-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="6dad9-104">Avage [Exchange'i administraatori center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="6dad9-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="6dad9-105">Mine **meilivoo** \> **aktsepteeritud domeenid**, valige aktsepteeritud ja klõpsake siis nuppu **Redigeeri**.</span><span class="sxs-lookup"><span data-stu-id="6dad9-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="6dad9-106">Atribuutide lehekülg avaneb, kui domeeni tüüp väärtuseks **Authoritative**, muutke **sisemiseks** vahedomeeniks ja klõpsake siis nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="6dad9-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="6dad9-107">Kui välised saatjad saavad viga, **teil ei ole õigust (550 5.7.13)**, käivitage järgmine käsk [Exchange Online PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) näha ühiskausta anonüümsete kasutajate õigused:</span><span class="sxs-lookup"><span data-stu-id="6dad9-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="6dad9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Näiteks `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="6dad9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="6dad9-109">Väliskasutajatele tuleks saada-seda ühiskausta, lisada CreateItems juurdepääs otse kasutaja Anonymous.</span><span class="sxs-lookup"><span data-stu-id="6dad9-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="6dad9-110">Näiteks `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="6dad9-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
