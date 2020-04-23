---
title: 1554 Winsock tõrge 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766165"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="82791-102">Winsock tõrge 10061</span><span class="sxs-lookup"><span data-stu-id="82791-102">Winsock error 10061</span></span>

<span data-ttu-id="82791-103">See tõrkekood tähendab, et Microsoft ei saa luua TCP pesa (ühendus) Target hosti.</span><span class="sxs-lookup"><span data-stu-id="82791-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="82791-104">Selle tõrke kõige tõenäolisem põhjus on tulemüüri konfiguratsiooniga seotud probleem.</span><span class="sxs-lookup"><span data-stu-id="82791-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="82791-105">Probleemi lahendamiseks kontrollige järgmisi sätteid.</span><span class="sxs-lookup"><span data-stu-id="82791-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="82791-106">Kontrollige oma tulemüüri konfiguratsiooni teavet [Microsoft 365 URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="82791-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="82791-107">Kui tõrge on seotud Exchange Online Protection (EOP), peaks olema varem teatatud muutus [Exchange Online Protection IP-aadressid](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="82791-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="82791-108">Veenduge, et teie Interneti-teenuse pakkuja (ISP) ei blokeeri porti.</span><span class="sxs-lookup"><span data-stu-id="82791-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="82791-109">Kontrollige oma konnektorite nutikat hosti ja sihtserveri sätteid.</span><span class="sxs-lookup"><span data-stu-id="82791-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="82791-110">Pange tähele, et Microsoft 365 ei blokeeri *sissetulevad* ühendused sel viisil.</span><span class="sxs-lookup"><span data-stu-id="82791-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
