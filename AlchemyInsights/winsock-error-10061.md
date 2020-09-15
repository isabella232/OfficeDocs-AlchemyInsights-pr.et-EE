---
title: 1554 Winsocki tõrge 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698858"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="c85b1-102">Winsocki tõrge 10061</span><span class="sxs-lookup"><span data-stu-id="c85b1-102">Winsock error 10061</span></span>

<span data-ttu-id="c85b1-103">See tõrkekood tähendab seda, et Microsoft ei suutnud luua Target hostiga TCP-liidest (ühendust).</span><span class="sxs-lookup"><span data-stu-id="c85b1-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="c85b1-104">Selle tõrke kõige tõenäolisem põhjus on probleem tulemüüri konfiguratsiooniga.</span><span class="sxs-lookup"><span data-stu-id="c85b1-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="c85b1-105">Probleemi lahendamiseks vaadake järgmisi sätteid.</span><span class="sxs-lookup"><span data-stu-id="c85b1-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="c85b1-106">Tulemüüri konfiguratsiooni kinnitamine [Microsoft 365 URL-ide ja IP-aadresside vahemikega](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) seotud teabega</span><span class="sxs-lookup"><span data-stu-id="c85b1-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="c85b1-107">Kui tõrkeks on Exchange Online ' i kaitse (EOP), oleks pidanud eelnevalt olema teatatud [Exchange Online ' i kaitse IP-aadresside](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)muutmisest.</span><span class="sxs-lookup"><span data-stu-id="c85b1-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="c85b1-108">Veenduge, et teie Interneti-teenuse pakkuja (ISP) ei blokeeriks porti.</span><span class="sxs-lookup"><span data-stu-id="c85b1-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="c85b1-109">Kontrollige, kas konnektorid on nutikad Host ja Target serveri sätted.</span><span class="sxs-lookup"><span data-stu-id="c85b1-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="c85b1-110">Pange tähele, et Microsoft 365 ei blokeeri sel viisil *sissetulevaid* ühendusi.</span><span class="sxs-lookup"><span data-stu-id="c85b1-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
